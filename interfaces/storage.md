# storage

## Implements

* `files`

## Configuration

### url

Where the contents of this storage instance reside.

Examples:

* file://server/path
* nfs://server/path

## Interface

### mount(mountpoint)

Ensure that the contents of this storage instance are mounted to `mountpoint` on the running host.

### umount(mountpoint)

Unmount the storage from `mountpoint` on the running host.

## Notes

Any services depending on a `storage` with a file:// URL must reside on the same host.
