

- Foundation
- FileWrapper
-  addFileWrapper(\_:) 

Instance Method

# addFileWrapper(\_:)

Adds a child file wrapper to the receiver, which must be a directory file wrapper.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addFileWrapper(_ child: FileWrapper) -> String
```

## Parameters 

`child`  

File wrapper to add to the directory.

## Return Value

Dictionary key used to store `fileWrapper` in the directory’s list of file wrappers. The dictionary key is a unique filename, which is the same as the passed-in file wrapper’s preferred filename unless that name is already in use as a key in the directory’s dictionary of children. See Accessing File Wrapper Identities in File System Programming Guide for more information about the file-wrapper list structure.

## Discussion

Use this method to add an existing file wrapper as a child of a directory file wrapper. If the file wrapper does not have a preferred filename, set the preferredFilename property to give it one before calling addFileWrapper(_:). To create a new file wrapper and add it to a directory, use the addRegularFile(withContents:preferredFilename:) method.

### Special Considerations

This method raises `NSInternalInconsistencyException` if the receiver is not a directory file wrapper.

This method raises `NSInvalidArgumentException` if the child file wrapper doesn’t have a preferred name.

## See Also

### Related Documentation

var preferredFilename: String?

The preferred filename for the file wrapper object.

### Accessing File-Wrapper Information

var fileWrappers: [String : FileWrapper]?

The file wrappers contained by a directory file wrapper.

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

func symbolicLinkDestination() -> String

Provides the pathname referenced by the file wrapper object, which must be a symbolic-link file wrapper.

Deprecated

var symbolicLinkDestinationURL: URL?

The URL referenced by the file wrapper object, which must be a symbolic-link file wrapper.

