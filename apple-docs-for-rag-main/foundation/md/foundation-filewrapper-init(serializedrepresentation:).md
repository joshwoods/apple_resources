

- Foundation
- FileWrapper
-  init(serializedRepresentation:) 

Initializer

# init(serializedRepresentation:)

Initializes the receiver as a regular-file file wrapper from given serialized data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(serializedRepresentation serializeRepresentation: Data)
```

## Parameters 

`serializeRepresentation`  

Serialized representation of a file wrapper in the format used for the `NSFileContentsPboardType` pasteboard type. Data of this format is returned by such methods as serializedRepresentation and rtfd(from:documentAttributes:) (NSAttributedString).

## Return Value

Regular-file file wrapper initialized from `serializedRepresentation`.

## Discussion

The file wrapper is not associated with a file-system node until you save it using write(to:options:originalContentsURL:).

## See Also

### Related Documentation

var preferredFilename: String?

The preferred filename for the file wrapper object.

var filename: String?

The filename of the file wrapper object

var fileAttributes: [String : Any]

A dictionary of file attributes.

### Creating File Wrappers

init(url: URL, options: FileWrapper.ReadingOptions) throws

Initializes a file wrapper instance whose kind is determined by the type of file-system node located by the URL.

convenience init?(path: String)

Initializes a file wrapper instance whose kind is determined by the type of file-system node located by the path.

Deprecated

init(directoryWithFileWrappers: [String : FileWrapper])

Initializes the receiver as a directory file wrapper, with a given file-wrapper list.

init(regularFileWithContents: Data)

Initializes the receiver as a regular-file file wrapper.

convenience init(symbolicLinkWithDestination: String)

Initializes the receiver as a symbolic-link file wrapper.

Deprecated

init(symbolicLinkWithDestinationURL: URL)

Initializes the receiver as a symbolic-link file wrapper that links to a specified file.

