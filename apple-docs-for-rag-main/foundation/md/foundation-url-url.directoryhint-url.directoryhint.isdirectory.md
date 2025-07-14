

- Foundation
- URL
- URL.DirectoryHint
-  URL.DirectoryHint.isDirectory 

Case

# URL.DirectoryHint.isDirectory

A hint that specifies that a given path is a directory.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
case isDirectory
```

## See Also

### Hints

case notDirectory

A hint that specifies that a given path isn’t a directory.

case checkFileSystem

A hint that directs a URL call to consult the file system to determine whether the path references a directory.

case inferFromPath

A hint that directs a URL call to infer whether a path references a directory based on whether it has a trailing slash.

