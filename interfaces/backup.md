# backup

## Depends

* `storage` (1): stores the backup

## Uses

* `files` (N): provides files to backup

## Interface

### backup(files, storage, path)

Make a backup of the files managed by `files` to `storage` at `path`.

### restore(files, storage, path)

Restore the freshest available backup from `storage` at `path` and push the result to `files`.
