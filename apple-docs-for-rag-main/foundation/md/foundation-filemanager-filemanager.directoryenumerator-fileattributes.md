

- Foundation
- FileManager
- FileManager.DirectoryEnumerator
-  fileAttributes 

Instance Property

# fileAttributes

A dictionary with the attributes of the most recently returned file or subdirectory (as referenced by the pathname).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var fileAttributes: [FileAttributeKey : Any]? { get }
```

## Discussion

See the description of the fileAttributes(atPath:traverseLink:) method of FileManager for details on obtaining the attributes from the dictionary.

## See Also

### Getting File and Directory Attributes

var directoryAttributes: [FileAttributeKey : Any]?

A dictionary with the attributes of the directory at which enumeration started.

var level: Int

The number of levels deep the current object is in the directory hierarchy being enumerated.

