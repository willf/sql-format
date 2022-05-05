# SQL-FORMAT

## Installation

```bash
poetry install
```

## Running

```bash
❯ script/sql-format --help
usage: sql-format [-h] [-f FILE] [-kc KEYWORD_CASE] [-ic IDENTIFIER_CASE] [-sc STRIP_COMMENTS] [-ri REINDENT] [-ra REINDENT_ALIGNED]
                  [-us USE_SPACE_AROUND_OPERATORS] [-it INDENT_TABS] [-iw INDENT_WIDTH] [-wa WRAP_AFTER] [-of OUTPUT_FORMAT] [-cf COMMA_FIRST]

Format SQL files

optional arguments:
  -h, --help            show this help message and exit
  -f FILE, --file FILE  SQL file to format. Default: stdin
  -kc KEYWORD_CASE, --keyword_case KEYWORD_CASE
                        Changes how keywords are formatted. Allowed values are “upper”, “lower” and “capitalize”. Default is “upper”.
  -ic IDENTIFIER_CASE, --identifier_case IDENTIFIER_CASE
                        Changes how identifiers are formatted. Allowed values are “upper”, “lower”, and “capitalize”. Default is “lower”.
  -sc STRIP_COMMENTS, --strip_comments STRIP_COMMENTS
                        If True comments are removed from the statements. Default is False.
  -ri REINDENT, --reindent REINDENT
                        If True the indentations of the statements are changed. Default is True.
  -ra REINDENT_ALIGNED, --reindent_aligned REINDENT_ALIGNED
                        If True the indentations of the statements are changed, and statements are aligned by keywords. Default is False.
  -us USE_SPACE_AROUND_OPERATORS, --use_space_around_operators USE_SPACE_AROUND_OPERATORS
                        If True spaces are used around all operators. Default is False.
  -it INDENT_TABS, --indent_tabs INDENT_TABS
                        If True tabs instead of spaces are used for indentation. Default is False.
  -iw INDENT_WIDTH, --indent_width INDENT_WIDTH
                        The width of the indentation. Default is 2.
  -wa WRAP_AFTER, --wrap_after WRAP_AFTER
                        The column limit (in characters) for wrapping comma-separated lists. If unspecified, it puts every item in the list on its own line.
                        Default is False.
  -of OUTPUT_FORMAT, --output_format OUTPUT_FORMAT
                        If given the output is additionally formatted to be used as a variable in a programming language. Allowed values are “sql”, “python”
                        and “php”. Default is “sql”.
  -cf COMMA_FIRST, --comma_first COMMA_FIRST
                        If True comma-first notation for column names is used. Default is False.
```
