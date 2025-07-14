

- FSKit
- FSVolume
- FSVolume.AccessMask
-  listDirectory 

Type Property

# listDirectory

The file system allows listing directory contents.

macOS 15.4+

``` source
static var listDirectory: FSVolume.AccessMask { get }
```

## See Also

### Declaring directory access

static var addFile: FSVolume.AccessMask

The file system allows adding files.

static var addSubdirectory: FSVolume.AccessMask

The file system allows adding subdirectories.

static var deleteChild: FSVolume.AccessMask

The file system allows deleting subdirectories.

static var search: FSVolume.AccessMask

The file system allows searching files.

