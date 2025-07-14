

- Foundation
- FileWrapper
-  init(directoryWithFileWrappers:) 

Initializer

# init(directoryWithFileWrappers:)

Initializes the receiver as a directory file wrapper, with a given file-wrapper list.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(directoryWithFileWrappers childrenByPreferredName: [String : FileWrapper])
```

## Parameters 

`childrenByPreferredName`  

Key-value dictionary of file wrappers with which to initialize the receiver. The dictionary must contain entries whose values are the file wrappers that are to become children and whose keys are filenames. See Accessing File Wrapper Identities in File System Programming Guide for more information about the file-wrapper list structure.

## Return Value

Initialized file wrapper for `fileWrappers`.

## Discussion

After initialization, the file wrapper is not associated with a file-system node until you save it using write(to:options:originalContentsURL:).

The receiver is initialized with open permissions: anyone can read, write, or modify the directory on disk.

If any file wrapper in the directory doesn’t have a preferred filename, its preferred name is automatically set to its corresponding key in the `childrenByPreferredName` dictionary.

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

init(regularFileWithContents: Data)

Initializes the receiver as a regular-file file wrapper.

convenience init(symbolicLinkWithDestination: String)

Initializes the receiver as a symbolic-link file wrapper.

Deprecated

init(symbolicLinkWithDestinationURL: URL)

Initializes the receiver as a symbolic-link file wrapper that links to a specified file.

init?(serializedRepresentation: Data)

Initializes the receiver as a regular-file file wrapper from given serialized data.

