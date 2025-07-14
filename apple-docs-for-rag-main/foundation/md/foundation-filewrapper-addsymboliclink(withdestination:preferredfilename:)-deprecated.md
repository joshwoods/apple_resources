

- Foundation
- FileWrapper
-  addSymbolicLink(withDestination:preferredFilename:) Deprecated

Instance Method

# addSymbolicLink(withDestination:preferredFilename:)

Creates a symbolic-link file wrapper pointing to a given file-system node and adds it to the receiver, which must be a directory file wrapper.

macOS 10.0–10.10Deprecated

``` source
func addSymbolicLink(
    withDestination path: String,
    preferredFilename filename: String
) -> String
```

Deprecated

Use addFileWrapper(_:) instead.

## Parameters 

`path`  

Pathname the new symbolic-link file wrapper is to reference.

`filename`  

Preferred filename for the new symbolic-link file wrapper.

## Return Value

Dictionary key used to store the new file wrapper in the directory’s list of file wrappers. See Accessing File Wrapper Identities in File System Programming Guide for more information.

## Discussion

Beginning with OS X v10.6, the preferred method of referring to files is with a `file://` URL. Instead of using this method, you can instantiate `NSFileWrapper` with one of the initializers, set its preferredFilename property if necessary, and pass the result to addFileWrapper(_:).

This method raises `NSInternalInconsistencyException` if the receiver is not a directory file wrapper.

This method raises `NSInvalidArgumentException` if you pass `nil` or an empty value for `preferredFilename`.

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

func keyForChildFileWrapper(FileWrapper) -> String?

Returns the dictionary key used by a directory to identify a given file wrapper.

func symbolicLinkDestination() -> String

Provides the pathname referenced by the file wrapper object, which must be a symbolic-link file wrapper.

Deprecated

var symbolicLinkDestinationURL: URL?

The URL referenced by the file wrapper object, which must be a symbolic-link file wrapper.

