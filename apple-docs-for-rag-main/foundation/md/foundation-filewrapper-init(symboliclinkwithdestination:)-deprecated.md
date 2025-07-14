

- Foundation
- FileWrapper
-  init(symbolicLinkWithDestination:) Deprecated

Initializer

# init(symbolicLinkWithDestination:)

Initializes the receiver as a symbolic-link file wrapper.

macOS 10.0–10.10Deprecated

``` source
convenience init(symbolicLinkWithDestination path: String)
```

Deprecated

Use init(symbolicLinkWithDestinationURL:) instead.

## Parameters 

`path`  

Pathname the receiver is to represent.

## Return Value

Initialized symbolic-link file wrapper referencing `node`.

## Discussion

The receiver is not associated to a file-system node until you save it using write(toFile:atomically:updateFilenames:). It’s also initialized with open permissions; anyone can read or write the disk representations it saves.

### Special Considerations

Beginning with OS X v10.6, the preferred method of referring to files is with a `file://` URL. Therefore, this method has been deprecated in favor of init(symbolicLinkWithDestinationURL:).

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

init(symbolicLinkWithDestinationURL: URL)

Initializes the receiver as a symbolic-link file wrapper that links to a specified file.

init?(serializedRepresentation: Data)

Initializes the receiver as a regular-file file wrapper from given serialized data.

