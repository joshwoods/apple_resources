

- FSKit
- FSVolume
-  FSVolume.AccessMask 

Structure

# FSVolume.AccessMask

A bitmask of access rights.

macOS 15.4+

``` source
struct AccessMask
```

## Topics

### Declaring read and write access

static var readData: FSVolume.AccessMask

The file system allows reading data.

static var writeData: FSVolume.AccessMask

The file system allows writing data.

### Declaring directory access

static var listDirectory: FSVolume.AccessMask

The file system allows listing directory contents.

static var addFile: FSVolume.AccessMask

The file system allows adding files.

static var addSubdirectory: FSVolume.AccessMask

The file system allows adding subdirectories.

static var deleteChild: FSVolume.AccessMask

The file system allows deleting subdirectories.

static var search: FSVolume.AccessMask

The file system allows searching files.

### Declaring file maniulation access

static var execute: FSVolume.AccessMask

The file system allows file executuion.

static var delete: FSVolume.AccessMask

The file system allows deleting a file.

static var appendData: FSVolume.AccessMask

The file system allows appending data to a file.

### Declaring attribute access

static var readAttributes: FSVolume.AccessMask

The file system allows reading file attributes.

static var writeAttributes: FSVolume.AccessMask

The file system allows writing file attributes.

static var readXattr: FSVolume.AccessMask

The file system allows reading extended file attributes.

static var writeXattr: FSVolume.AccessMask

The file system allows writing extended file attributes.

static var readSecurity: FSVolume.AccessMask

The file system allows reading a file’s security descriptors.

static var writeSecurity: FSVolume.AccessMask

The file system allows writing a file’s security descriptors.

### Ownership access

static var takeOwnership: FSVolume.AccessMask

The file system allows taking ownership of a file.

### Working with raw values

init(rawValue: UInt)

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Checking access

func checkAccess(to: FSItem, requestedAccess: FSVolume.AccessMask, replyHandler: (Bool, (any Error)?) -> Void)

Checks whether the file system allows access to the given item.

**Required**

