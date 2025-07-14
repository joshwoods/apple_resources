

- Foundation
- FileManager
-  string(withFileSystemRepresentation:length:) 

Instance Method

# string(withFileSystemRepresentation:length:)

Returns an NSString object whose contents are derived from the specified C-string path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func string(
    withFileSystemRepresentation str: UnsafePointer,
    length len: Int
) -> String
```

## Parameters 

`str`  

A C string representation of a pathname.

`len`  

The number of characters in `string`.

## Return Value

An NSString object converted from the C-string representation `string` with length `len` of a pathname in the current file system.

## Discussion

Use this method if your code receives paths as C strings from system routines.

## See Also

### Converting File Paths to Strings

func fileSystemRepresentation(withPath: String) -> UnsafePointer&lt;CChar>

Returns a C-string representation of a given path that properly encodes Unicode strings for use by the file system.

