# NYT Sudoku Archive

This repository contains a daily archive of Sudoku puzzles extracted from [The New York Times](https://www.nytimes.com/puzzles/sudoku). The puzzles are stored in a custom **.sdk** text format, making them easy to parse, analyze, or import into Sudoku solvers and applications.

## 📂 Repository Structure

The files are organized in separate folders for each difficulty level (easy, medium, and hard) using the following naming convention:

`nyt-sudoku-{difficulty}-{YYYY-MM-DD}.sdk`

**Examples:**
* `nyt-sudoku-easy-2026-02-04.sdk`
* `nyt-sudoku-medium-2026-02-04.sdk`
* `nyt-sudoku-hard-2026-02-04.sdk`

## 📄 SDK File Format Specification

Each `.sdk` file is a plain text file containing metadata headers followed by the puzzle grid.

### Puzzle Grid
The puzzle is represented as 9 lines of text.
* Digits **1-9** represent pre-filled clues.
* Dots **`.`** represent empty cells.
* There are no spaces or separators between cells.

### Example File Content
```text
#SNew York Times
#B2026-02-04
#LEasy
#DThe New York Times Easy Sudoku for 2026-02-04
#CNYT Puzzle Id: 150919
158.....2
7..78254.
.2..371..
...51..8.
38..4.26.
5.64.87..
...3....6
2.7..14.3
.6.1.9..5
