

- Foundation
- FileWrapper
-  keyForChildFileWrapper(\_:) 

Instance Method

# keyForChildFileWrapper(\_:)

Returns the dictionary key used by a directory to identify a given file wrapper.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func keyForChildFileWrapper(_ child: FileWrapper) -> String?
```

## Parameters 

`child`  

The child file wrapper for which you want the key.

## Return Value

Dictionary key used to store the file wrapper in the directory’s list of file wrappers. The dictionary key is a unique filename, which may not be the same as the passed-in file wrapper’s preferred filename if more than one file wrapper in the directory’s dictionary of children has the same preferred filename. See Accessing File Wrapper Identities in File System Programming Guide for more information about the file-wrapper list structure. Returns `nil` if the file wrapper specified in `child` is not a child of the directory.

## Discussion

This method raises `NSInternalInconsistencyException` if the receiver is not a directory file wrapper.

## See Also

### Related Documentation

var filename: String?

The filename of the file wrapper object

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

func symbolicLinkDestination() -> String

Provides the pathname referenced by the file wrapper object, which must be a symbolic-link file wrapper.

Deprecated

var symbolicLinkDestinationURL: URL?

The URL referenced by the file wrapper object, which must be a symbolic-link file wrapper.

