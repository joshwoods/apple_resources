

- Foundation
- URL
-  init(\_:) Deprecated

Initializer

# init(\_:)

Creates a file URL that references the local file or directory at the file path you specify.

iOS 14.0–16.0DeprecatediPadOS 14.0–16.0DeprecatedMac Catalyst 14.0–16.0DeprecatedmacOS 11.0–13.0DeprecatedtvOS 14.0–16.0DeprecatedwatchOS 7.0–9.0Deprecated

``` source
init?(_ path: FilePath)
```

## Parameters 

`path`  

The location in the file system.

## Discussion

This method may perform file system I/O to determine if the path is to a directory. If you know the path is to a directory, use init(_:isDirectory:) to avoid the file system I/O.

## See Also

### Creating a file URL from a file path

init?(FilePath, isDirectory: Bool)

Creates a file URL that references the local file or directory at the file path you specify.

Deprecated

struct FilePath

Represents a location in the file system.

