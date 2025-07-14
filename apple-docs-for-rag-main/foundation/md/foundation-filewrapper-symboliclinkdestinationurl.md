

- Foundation
- FileWrapper
-  symbolicLinkDestinationURL 

Instance Property

# symbolicLinkDestinationURL

The URL referenced by the file wrapper object, which must be a symbolic-link file wrapper.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var symbolicLinkDestinationURL: URL? { get }
```

## Discussion

This property may contain `nil` if the user modifies the symbolic link after you call read(from:options:) or init(url:options:) but before FileWrapper has read the contents of the link. Use the immediate reading option to reduce the likelihood of that problem.

### Special Considerations

This property raises `NSInternalInconsistencyException` if the file wrapper object is not a symbolic-link file wrapper.

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

func symbolicLinkDestination() -> String

Provides the pathname referenced by the file wrapper object, which must be a symbolic-link file wrapper.

Deprecated

