

- Foundation
- FileWrapper
-  init(symbolicLinkWithDestinationURL:) 

Initializer

# init(symbolicLinkWithDestinationURL:)

Initializes the receiver as a symbolic-link file wrapper that links to a specified file.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(symbolicLinkWithDestinationURL url: URL)
```

## Parameters 

`url`  

URL of the file the file wrapper is to reference.

## Return Value

Initialized symbolic-link file wrapper referencing `url`.

## Discussion

The file wrapper is not associated with a file-system node until you save it using write(to:options:originalContentsURL:).

The file wrapper is initialized with open permissions: anyone can modify or read the file reference. .

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

init?(serializedRepresentation: Data)

Initializes the receiver as a regular-file file wrapper from given serialized data.

