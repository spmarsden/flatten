# Flatten
Takes a directory tree and flattens it into a single directory.

## Example

Running `flatten ./dir0` where the directory structure looks like this:

    ./
        dir0/
            dir01/
                dir010/
                    file0100
                dir011/
                file010
            dir02/
                file020
                file021

would result in the following structure:

    ./
        dir0/
            dir01_dir010_file0100
            dir01_file010
            dir02_file020
            dir02_file021

## Exit Codes

| Code | Meaning                |
| ---- | ---------------------- |
| 0    | Completed Successfully |
| 1    | Unused                 |
| 2    | Invalid Arguments      |
| 3    | Move Error             |