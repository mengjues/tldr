# find

> Find files under the given directory tree, recursively

- find files by extension

`find {{root_path}} -name {{'*.py'}}`

- run a command for each file
- use {} within the command to access the filename

`find {{root_path}} -name {{'*.py'}} -exec {{command}} \;`

- find files modified since a certain time

`find {{root_path}} -name {{'*.py'}} -mtime {{-1d}}`

- remove files recursively

`find {{root_path}} -name {{'*.py'}} -exec rm {} \;`
