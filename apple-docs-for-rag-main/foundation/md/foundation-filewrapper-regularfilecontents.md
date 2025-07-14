

- Foundation
- FileWrapper
-  regularFileContents 

Instance Property

# regularFileContents

The contents of the file-system node associated with a regular-file file wrapper.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var regularFileContents: Data? { get }
```

## Discussion

This property may contain `nil` if the user modifies the file after you call read(from:options:) or init(url:options:) but before FileWrapper has read the contents of the file. Use the immediate reading option to reduce the likelihood of that problem.

### Special Considerations

This property raises `NSInternalInconsistencyException` if the file wrapper object is not a regular-file file wrapper.

## See Also

### Related Documentation

func read(from: URL, options: FileWrapper.ReadingOptions) throws

Recursively rereads the entire contents of a file wrapper from the specified location on disk.

init(regularFileWithContents: Data)

Initializes the receiver as a regular-file file wrapper.

### Accessing Files

var filename: String?

The filename of the file wrapper object

var preferredFilename: String?

The preferred filename for the file wrapper object.

var fileAttributes: [String : Any]

A dictionary of file attributes.

