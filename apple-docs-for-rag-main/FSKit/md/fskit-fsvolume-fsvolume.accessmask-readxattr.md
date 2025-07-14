

- FSKit
- FSVolume
- FSVolume.AccessMask
-  readXattr 

Type Property

# readXattr

The file system allows reading extended file attributes.

macOS 15.4+

``` source
static var readXattr: FSVolume.AccessMask { get }
```

## See Also

### Declaring attribute access

static var readAttributes: FSVolume.AccessMask

The file system allows reading file attributes.

static var writeAttributes: FSVolume.AccessMask

The file system allows writing file attributes.

static var writeXattr: FSVolume.AccessMask

The file system allows writing extended file attributes.

static var readSecurity: FSVolume.AccessMask

The file system allows reading a file’s security descriptors.

static var writeSecurity: FSVolume.AccessMask

The file system allows writing a file’s security descriptors.

