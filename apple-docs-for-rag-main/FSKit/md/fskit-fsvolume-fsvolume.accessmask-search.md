

- FSKit
- FSVolume
- FSVolume.AccessMask
-  search 

Type Property

# search

The file system allows searching files.

macOS 15.4+

``` source
static var search: FSVolume.AccessMask { get }
```

## See Also

### Declaring directory access

static var listDirectory: FSVolume.AccessMask

The file system allows listing directory contents.

static var addFile: FSVolume.AccessMask

The file system allows adding files.

static var addSubdirectory: FSVolume.AccessMask

The file system allows adding subdirectories.

static var deleteChild: FSVolume.AccessMask

The file system allows deleting subdirectories.

