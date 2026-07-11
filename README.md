# Google Sheets Formulas

A reference collection of Google Sheets formulas built to solve recurring spreadsheet tasks. Each formula file is plain text containing the formula plus inline `//` comments explaining how to use it (Sheets doesn't support real comments, so these are stripped out before pasting into a cell).

## Formulas

| File | What it does |
|---|---|
| [deadline-formula.txt](./formulas/deadline-formula.txt) | Calculates a document submission deadline from a base date, case category, and rush-fee tier using nested `IFS`/`WORKDAY` logic. Category/package labels are genericized placeholders. |
| [occurrences-in-a-month.txt](./formulas/occurrences-in-a-month.txt) | Counts how many dates in a range fall in a given month, using `COUNTIF` + `ARRAYFORMULA(MONTH(...))`. |
| [transfer-data-by-year.txt](./formulas/transfer-data-by-year.txt) | Pulls and sorts rows from another sheet (via `IMPORTRANGE`) into a per-year summary tab, filtering by year and handling blanks with `IFERROR`. |

## Usage

Open the `.txt` file for the formula you need, copy the formula (the line(s) starting with `=`), and paste into a Google Sheets cell — then adjust the cell references / placeholder tokens (like `**:*` or `************`) to match your sheet.
