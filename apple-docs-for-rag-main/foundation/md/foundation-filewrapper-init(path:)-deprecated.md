

- Foundation
- FileWrapper
-  init(path:) Deprecated

Initializer

# init(path:)

Initializes a file wrapper instance whose kind is determined by the type of file-system node located by the path.

macOS 10.0–10.10Deprecated

``` source
convenience init?(path: String)
```

Deprecated

Use init(url:options:) instead.

## Parameters 

`path`  

Pathname of the file-system node the file wrapper is to represent.

## Return Value

File wrapper for `node`.

## Discussion

If `node` is a directory, this method recursively creates file wrappers for each node within that directory.

### Special Considerations

Beginning with OS X v10.6, the preferred method of referring to files is with a `file://` URL. Therefore, this method has been deprecated in favor of init(url:options:).

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

init(directoryWithFileWrappers: [String : FileWrapper])

Initializes the receiver as a directory file wrapper, with a given file-wrapper list.

init(regularFileWithContents: Data)

Initializes the receiver as a regular-file file wrapper.

convenience init(symbolicLinkWithDestination: String)

Initializes the receiver as a symbolic-link file wrapper.

Deprecated

init(symbolicLinkWithDestinationURL: URL)

Initializes the receiver as a symbolic-link file wrapper that links to a specified file.

init?(serializedRepresentation: Data)

Initializes the receiver as a regular-file file wrapper from given serialized data.

