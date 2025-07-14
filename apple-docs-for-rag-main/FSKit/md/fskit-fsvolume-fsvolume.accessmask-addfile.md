

- FSKit
- FSVolume
- FSVolume.AccessMask
-  addFile 

Type Property

# addFile

The file system allows adding files.

macOS 15.4+

``` source
static var addFile: FSVolume.AccessMask { get }
```

## See Also

### Declaring directory access

static var listDirectory: FSVolume.AccessMask

The file system allows listing directory contents.

static var addSubdirectory: FSVolume.AccessMask

The file system allows adding subdirectories.

static var deleteChild: FSVolume.AccessMask

The file system allows deleting subdirectories.

static var search: FSVolume.AccessMask

The file system allows searching files.

