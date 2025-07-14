

- Foundation
- FileWrapper
-  symbolicLinkDestination() Deprecated

Instance Method

# symbolicLinkDestination()

Provides the pathname referenced by the file wrapper object, which must be a symbolic-link file wrapper.

macOS 10.0–10.10Deprecated

``` source
func symbolicLinkDestination() -> String
```

Deprecated

Use symbolicLinkDestinationURL instead.

## Return Value

Pathname the file wrapper references (the destination of the symbolic link the file wrapper represents).

## Discussion

Beginning with OS X v10.6, the preferred method of referring to files is with a `file://` URL. Therefore, this method has been deprecated in favor of symbolicLinkDestinationURL.

This method raises `NSInternalInconsistencyException` if the receiver is not a symbolic-link file wrapper.

## See Also

### Accessing File-Wrapper Information

var fileWrappers: [String : FileWrapper]?

The file wrappers contained by a directory file wrapper.

func addFileWrapper(FileWrapper) -> String

Adds a child file wrapper to the receiver, which must be a directory file wrapper.

func removeFileWrapper(FileWrapper)

Removes a child file wrapper from the receiver, which must be a directory file wrapper.

func addFile(withPath: String) -> String

Creates a file wrapper from a given file-system node and adds it to the receiver, which must be a directory file wrapper.

Deprecated

func addRegularFile(withContents: Data, preferredFilename: String) -> String

Creates a regular-file file wrapper with the given contents and adds it to the receiver, which must be a directory file wrapper.

func addSymbolicLink(withDestination: String, preferredFilename: String) -> String

Creates a symbolic-link file wrapper pointing to a given file-system node and adds it to the receiver, which must be a directory file wrapper.

Deprecated

func keyForChildFileWrapper(FileWrapper) -> String?

Returns the dictionary key used by a directory to identify a given file wrapper.

var symbolicLinkDestinationURL: URL?

The URL referenced by the file wrapper object, which must be a symbolic-link file wrapper.

