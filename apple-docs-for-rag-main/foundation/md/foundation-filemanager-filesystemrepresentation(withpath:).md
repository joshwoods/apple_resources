

- Foundation
- FileManager
-  fileSystemRepresentation(withPath:) 

Instance Method

# fileSystemRepresentation(withPath:)

Returns a C-string representation of a given path that properly encodes Unicode strings for use by the file system.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func fileSystemRepresentation(withPath path: String) -> UnsafePointer
```

## Parameters 

`path`  

A string object containing a path to a file. This parameter must not be `nil` or contain the empty string.

## Return Value

A C-string representation of `path` that properly encodes Unicode strings for use by the file system.

## Discussion

Use this method if your code calls system routines that expect C-string path arguments. If you use the C string beyond the scope of the current autorelease pool, you must copy it.

This method raises an exception if `path` is `nil` or contains the empty string. This method also throws an exception if the conversion of the string fails.

## See Also

### Converting File Paths to Strings

func string(withFileSystemRepresentation: UnsafePointer&lt;CChar>, length: Int) -> String

Returns an NSString object whose contents are derived from the specified C-string path.

