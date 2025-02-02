# many-toon-cli
Download 18+ Manhwa from manytoon using async 
# Many-Toon CLI

A command-line tool for downloading 18+ manga efficiently.

## Description

The **Many-Toon CLI** tool allows users to search, download, and organize 18+ Manhwa chapters from the command line. With features to specify download ranges and custom paths, it's designed for quick and flexible usage.

## Installation

Install the CLI tool directly using:

```bash
pip install many-toon-cli
```

Alternatively, if you’re installing from source, navigate to the directory with the setup.py file and run:
```bash
pip install .
```

## Usage

To use the CLI, enter the following command format:
```bash
many-toon-cli "<manga_title>" [-c <start> <end>] [-p <path>] [-ip <input_pos>]
```
## Options
```bash 
[I] xxG(xxx) ~/many-toon-cli (main) > python manga.py -h           11:53:29
usage: manga.py [-h] [-c start end] [-p PATH] [-ip INPUT_POS] search_term

Search and download manga chapters.

positional arguments:
  search_term           Search term to find manga

options:
  -h, --help            show this help message and exit
  -c start end, --chapters start end
                        Chapter range to download (start end)
  -p PATH, --path PATH  Directory where the chapters will be downloaded
                        (default: current directory)
  -ip INPUT_POS, --input-pos INPUT_POS
                        Position of the manga in the list to select
                        automatically (1-based index)
```

## Example

Download chapters 1 through 5 of a manga titled "Secret Class" to a specific directory:

many-toon-cli "Secret Class" -c 1 5 -p /path/to/download


