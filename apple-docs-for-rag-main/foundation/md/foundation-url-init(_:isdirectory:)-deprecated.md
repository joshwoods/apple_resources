

- Foundation
- URL
-  init(\_:isDirectory:) Deprecated

Initializer

# init(\_:isDirectory:)

Creates a file URL that references the local file or directory at the file path you specify.

iOS 14.0–16.0DeprecatediPadOS 14.0–16.0DeprecatedMac Catalyst 14.0–16.0DeprecatedmacOS 11.0–13.0DeprecatedtvOS 14.0–16.0DeprecatedwatchOS 7.0–9.0Deprecated

``` source
init?(
    _ path: FilePath,
    isDirectory: Bool
)
```

Deprecated

Use init?(filePath:directoryHint:) instead

## Parameters 

`path`  

The location in the file system.

`isDirectory`  

A Boolean value that indicates whether the location is a directory.

## Discussion

Note

This method avoids file system I/O to determine if the path is to a directory. When you know that information, prefer this method to initializers without the parameter.

## See Also

### Creating a file URL from a file path

init?(FilePath)

Creates a file URL that references the local file or directory at the file path you specify.

Deprecated

struct FilePath

Represents a location in the file system.

