

- Foundation
- FileWrapper
-  read(from:options:) 

Instance Method

# read(from:options:)

Recursively rereads the entire contents of a file wrapper from the specified location on disk.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func read(
    from url: URL,
    options: FileWrapper.ReadingOptions = []
) throws
```

## Parameters 

`url`  

URL of the file-system node corresponding to the file wrapper.

`options`  

Option flags for reading the node located at `url`. See FileWrapper.ReadingOptions for possible values.

## Discussion

When reading a directory, children are added and removed as necessary to match the file system.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

var fileWrappers: [String : FileWrapper]?

The file wrappers contained by a directory file wrapper.

init(url: URL, options: FileWrapper.ReadingOptions) throws

Initializes a file wrapper instance whose kind is determined by the type of file-system node located by the URL.

var filename: String?

The filename of the file wrapper object

var fileAttributes: [String : Any]

A dictionary of file attributes.

func write(to: URL, options: FileWrapper.WritingOptions, originalContentsURL: URL?) throws

Recursively writes the entire contents of a file wrapper to a given file-system URL.

### Updating File Wrappers

func needsToBeUpdated(fromPath: String) -> Bool

Indicates whether the file wrapper needs to be updated to match a given file-system node.

Deprecated

func matchesContents(of: URL) -> Bool

Indicates whether the contents of a file wrapper matches a directory, regular file, or symbolic link on disk.

func update(fromPath: String) -> Bool

Updates the file wrapper to match a given file-system node.

Deprecated

