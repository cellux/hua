# files

## Interface

### pull(stream)

Create a .tar.gz of the managed files and pipe it to `stream`.

### push(stream)

Replace the managed files with the files from `stream` which arrive packed into a .tar.gz archive.
