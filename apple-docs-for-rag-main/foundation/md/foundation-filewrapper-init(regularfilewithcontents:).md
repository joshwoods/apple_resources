

- Foundation
- FileWrapper
-  init(regularFileWithContents:) 

Initializer

# init(regularFileWithContents:)

Initializes the receiver as a regular-file file wrapper.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(regularFileWithContents contents: Data)
```

## Parameters 

`contents`  

Contents of the file.

## Return Value

Initialized regular-file file wrapper containing `contents`.

## Discussion

After initialization, the file wrapper is not associated with a file-system node until you save it using write(to:options:originalContentsURL:).

The file wrapper is initialized with open permissions: anyone can write to or read the file wrapper.

## See Also

### Related Documentation

var preferredFilename: String?

The preferred filename for the file wrapper object.

var filename: String?

The filename of the file wrapper object

var fileAttributes: [String : Any]

A dictionary of file attributes.

var regularFileContents: Data?

The contents of the file-system node associated with a regular-file file wrapper.

### Creating File Wrappers

init(url: URL, options: FileWrapper.ReadingOptions) throws

Initializes a file wrapper instance whose kind is determined by the type of file-system node located by the URL.

convenience init?(path: String)

Initializes a file wrapper instance whose kind is determined by the type of file-system node located by the path.

Deprecated

init(directoryWithFileWrappers: [String : FileWrapper])

Initializes the receiver as a directory file wrapper, with a given file-wrapper list.

convenience init(symbolicLinkWithDestination: String)

Initializes the receiver as a symbolic-link file wrapper.

Deprecated

init(symbolicLinkWithDestinationURL: URL)

Initializes the receiver as a symbolic-link file wrapper that links to a specified file.

init?(serializedRepresentation: Data)

Initializes the receiver as a regular-file file wrapper from given serialized data.

