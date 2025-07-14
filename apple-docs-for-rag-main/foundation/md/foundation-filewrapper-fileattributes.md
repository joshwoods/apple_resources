

- Foundation
- FileWrapper
-  fileAttributes 

Instance Property

# fileAttributes

A dictionary of file attributes.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var fileAttributes: [String : Any] { get set }
```

## Discussion

The file attributes’ dictionary is the same format as that returned by attributesOfItem(atPath:) (`NSFileManager`).

## See Also

### Accessing Files

var filename: String?

The filename of the file wrapper object

var preferredFilename: String?

The preferred filename for the file wrapper object.

var regularFileContents: Data?

The contents of the file-system node associated with a regular-file file wrapper.

