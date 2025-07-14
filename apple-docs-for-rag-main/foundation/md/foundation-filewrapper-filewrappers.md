

- Foundation
- FileWrapper
-  fileWrappers 

Instance Property

# fileWrappers

The file wrappers contained by a directory file wrapper.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var fileWrappers: [String : FileWrapper]? { get }
```

## Discussion

The dictionary contains entries whose values are the file wrappers and whose keys are the unique filenames that have been assigned to each one. See Accessing File Wrapper Identities in File System Programming Guide for more information about the file-wrapper list structure.

This property may contain `nil` if the user modifies the directory after you call read(from:options:) or init(url:options:) but before FileWrapper has read the contents of the directory. Use the immediate reading option to reduce the likelihood of that problem.

### Special Considerations

This property raises `NSInternalInconsistencyException` if the file wrapper object is not a directory file wrapper.

## See Also

### Related Documentation

var filename: String?

The filename of the file wrapper object

### Accessing File-Wrapper Information

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

func symbolicLinkDestination() -> String

Provides the pathname referenced by the file wrapper object, which must be a symbolic-link file wrapper.

Deprecated

var symbolicLinkDestinationURL: URL?

The URL referenced by the file wrapper object, which must be a symbolic-link file wrapper.

