

- FSKit
- FSVolume
- FSVolume.AccessMask
-  deleteChild 

Type Property

# deleteChild

The file system allows deleting subdirectories.

macOS 15.4+

``` source
static var deleteChild: FSVolume.AccessMask { get }
```

## See Also

### Declaring directory access

static var listDirectory: FSVolume.AccessMask

The file system allows listing directory contents.

static var addFile: FSVolume.AccessMask

The file system allows adding files.

static var addSubdirectory: FSVolume.AccessMask

The file system allows adding subdirectories.

static var search: FSVolume.AccessMask

The file system allows searching files.

