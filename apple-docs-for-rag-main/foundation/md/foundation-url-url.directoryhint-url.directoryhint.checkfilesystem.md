

- Foundation
- URL
- URL.DirectoryHint
-  URL.DirectoryHint.checkFileSystem 

Case

# URL.DirectoryHint.checkFileSystem

A hint that directs a URL call to consult the file system to determine whether the path references a directory.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
case checkFileSystem
```

## See Also

### Hints

case isDirectory

A hint that specifies that a given path is a directory.

case notDirectory

A hint that specifies that a given path isn’t a directory.

case inferFromPath

A hint that directs a URL call to infer whether a path references a directory based on whether it has a trailing slash.

