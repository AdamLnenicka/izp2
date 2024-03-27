Command-line tool designed for manipulating and processing tabular data. It provides functionalities for modifying the structure of tables, selecting rows, and processing data within cells

## Usage

The "sheet" tool supports two main modes of operation: adjusting table structure and data processing. Additionally, it allows for selecting specific rows for processing.

### Adjusting Table Structure

The following commands are available for modifying the structure of the table:

- `irow R`: Insert a row before row R (R > 0).
- `arow`: Append a new row to the end of the table.
- `drow R`: Delete row number R (R > 0).
- `drows N M`: Delete rows N through M (N <= M).
- `icol C`: Insert an empty column before column C.
- `acol`: Append an empty column after the last column.
- `dcol C`: Delete column number C.
- `dcols N M`: Delete columns N through M (N <= M).

### Data Processing

The "sheet" tool provides various commands for processing data within cells:

- `cset C STR`: Set a string STR in the cell of column C.
- `tolower C`: Convert the string in column C to lowercase.
- `toupper C`: Convert the string in column C to uppercase.
- `round C`: Round the number in column C to the nearest integer.
- `int C`: Remove the decimal part of the number in column C.
- `copy N M`: Overwrite the contents of cells in column M with values from column N.
- `swap N M`: Swap the values of cells in columns N and M.
- `move N M`: Move column N before column M.

### Row Selection

The following commands allow for selecting specific rows for processing:

- `rows N M`: Process only rows N through M (N <= M).
- `beginswith C STR`: Process only rows where the content of the cell in column C begins with the string STR.
- `contains C STR`: Process only rows where the cells in column C contain the string STR.

## Limitations

This project has the following limitations:

- The use of dynamic memory allocation functions (`malloc` and `free`) is prohibited.
- File I/O functions (`fopen`, `fclose`, `fscanf`, etc.) should not be used.
- Sorting and searching functions (`qsort`, `lsearch`, `bsearch`, `hsearch`) are not allowed.
- The `exit` function should not be used.

---

You can replace the placeholders (like `yourusername` in the clone URL) with your actual GitHub username and customize any other parts of the documentation as needed.
