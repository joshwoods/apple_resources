

- FSKit
- FSVolume
- FSVolume.AccessMask
-  addSubdirectory 

Type Property

# addSubdirectory

The file system allows adding subdirectories.

macOS 15.4+

``` source
static var addSubdirectory: FSVolume.AccessMask { get }
```

## See Also

### Declaring directory access

static var listDirectory: FSVolume.AccessMask

The file system allows listing directory contents.

static var addFile: FSVolume.AccessMask

The file system allows adding files.

static var deleteChild: FSVolume.AccessMask

The file system allows deleting subdirectories.

static var search: FSVolume.AccessMask

The file system allows searching files.

