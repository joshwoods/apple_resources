

- Foundation
- FileWrapper
-  isDirectory 

Instance Property

# isDirectory

This property contains a boolean value indicating whether the file wrapper is a directory file wrapper.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isDirectory: Bool { get }
```

## Discussion

This property will contain YES when the file wrapper is a directory file wrapper, otherwise it contains NO.

Note

Invocations of read(from:options:) may change the value of this property, if the type of the file on disk has changed.

## See Also

### Querying File Wrappers

var isRegularFile: Bool

This property contains a boolean value that indicates whether the file wrapper object is a regular-file.

var isSymbolicLink: Bool

A boolean that indicates whether the file wrapper object is a symbolic-link file wrapper.

