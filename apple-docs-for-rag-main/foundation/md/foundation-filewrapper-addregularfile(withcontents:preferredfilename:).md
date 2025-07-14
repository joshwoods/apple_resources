

- Foundation
- FileWrapper
-  addRegularFile(withContents:preferredFilename:) 

Instance Method

# addRegularFile(withContents:preferredFilename:)

Creates a regular-file file wrapper with the given contents and adds it to the receiver, which must be a directory file wrapper.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addRegularFile(
    withContents data: Data,
    preferredFilename fileName: String
) -> String
```

## Parameters 

`data`  

Contents for the new regular-file file wrapper.

`fileName`  

Preferred filename for the new regular-file file wrapper.

## Return Value

Dictionary key used to store the new file wrapper in the directory’s list of file wrappers. The dictionary key is a unique filename, which is the same as the passed-in file wrapper’s preferred filename unless that name is already in use as a key in the directory’s dictionary of children. See Accessing File Wrapper Identities in File System Programming Guide for more information about the file-wrapper list structure.

## Discussion

This is a convenience method. The default implementation allocates a new file wrapper, initializes it with init(regularFileWithContents:), set its preferredFilename property, adds it to the directory with addFileWrapper(_:), and returns what addFileWrapper(_:) returned.

### Special Considerations

This method raises `NSInternalInconsistencyException` if the receiver is not a directory file wrapper.

This method raises `NSInvalidArgumentException` if you pass `nil` or an empty value for `filename`.

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

