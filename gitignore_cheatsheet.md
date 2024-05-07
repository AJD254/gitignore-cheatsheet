## GitIgnore Cheatsheet

This cheatsheet provides a quick reference for common patterns used in `.gitignore` files to exclude files and folders from Git version control.

**Understanding Pattern Matching:**

* `*` (asterisk): Matches any number of characters (except `/`).
* `?` (question mark): Matches a single character.
* `[]` (brackets): Matches a character range (e.g., `[a-z]`).
* `!` (exclamation mark): Negates a pattern.

**Common GitIgnore Rules:**

| Pattern                | Explanation/Matches                                                                         | Examples                                 |
|------------------------|-----------------------------------------------------------------------------------------------|---------------------------------------------|
| `*.log`                | Ignores all files with the `.log` extension                                                         | `debug.log`, `server.log`, `errors.log`       |
| `/path/to/file`        | Ignores a specific file at the given path                                                             | `/tmp/cache.txt`, `/config.ini`            |
| `/path/to/folder/`     | Ignores an entire folder and its contents                                                       | `/build/`, `/node_modules/`                  |
| `**/logs`              | Ignores all files and subfolders within the `logs` directory anywhere in the repository             | `/logs/debug.log`, `/logs/errors.log`      |
| `*.tmp`                | Ignores all files with the `.tmp` extension                                                         | `temp.txt`, `cache.tmp`                      |
| `*~`                  | Ignores backup files created by some editors                                                       | `file.txt~`                               |
| `#` (comment)          | Lines starting with `#` are ignored (add comments for clarity)                                    | # Ignore local configuration              |
| `!important.file`     | Negates the previous pattern, including the ignored file                                          | `.gitignore`, `important.log`                |


