

- Foundation
- FileWrapper
-  init(url:options:) 

Initializer

# init(url:options:)

Initializes a file wrapper instance whose kind is determined by the type of file-system node located by the URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    url: URL,
    options: FileWrapper.ReadingOptions = []
) throws
```

## Parameters 

`url`  

URL of the file-system node the file wrapper is to represent.

`options`  

Option flags for reading the node located at `url`. See FileWrapper.ReadingOptions for possible values.

## Return Value

File wrapper for the file-system node at `url`. May be a directory, file, or symbolic link, depending on what is located at the URL. Returns false (0) if reading is not successful.

## Discussion

If `url` is a directory, this method recursively creates file wrappers for each node within that directory. Use the fileWrappers property to get the file wrappers of the nodes contained by the directory.

Handling Errors in Swift

In Swift, this API is imported as an initializer and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

var fileWrappers: [String : FileWrapper]?

The file wrappers contained by a directory file wrapper.

var preferredFilename: String?

The preferred filename for the file wrapper object.

func read(from: URL, options: FileWrapper.ReadingOptions) throws

Recursively rereads the entire contents of a file wrapper from the specified location on disk.

var filename: String?

The filename of the file wrapper object

File System Programming Guide

var fileAttributes: [String : Any]

A dictionary of file attributes.

### Creating File Wrappers

convenience init?(path: String)

Initializes a file wrapper instance whose kind is determined by the type of file-system node located by the path.

Deprecated

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

