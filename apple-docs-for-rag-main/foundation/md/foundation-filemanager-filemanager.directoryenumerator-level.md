

- Foundation
- FileManager
- FileManager.DirectoryEnumerator
-  level 

Instance Property

# level

The number of levels deep the current object is in the directory hierarchy being enumerated.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var level: Int { get }
```

## Discussion

The number of levels, with the directory passed to enumeratorAtURL:includingPropertiesForKeys:options:errorHandler: (`NSFileManager`) considered to be level `0`.

## See Also

### Getting File and Directory Attributes

var directoryAttributes: [FileAttributeKey : Any]?

A dictionary with the attributes of the directory at which enumeration started.

var fileAttributes: [FileAttributeKey : Any]?

A dictionary with the attributes of the most recently returned file or subdirectory (as referenced by the pathname).

