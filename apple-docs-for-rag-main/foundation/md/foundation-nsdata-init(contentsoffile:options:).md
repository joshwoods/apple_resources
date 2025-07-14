

- Foundation
- NSData
-  init(contentsOfFile:options:) 

Initializer

# init(contentsOfFile:options:)

Initializes a data object with the content of the file at a given path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    contentsOfFile path: String,
    options readOptionsMask: NSData.ReadingOptions = []
) throws
```

## Parameters 

`path`  

The absolute path of the file from which to read data.

`readOptionsMask`  

A mask that specifies options for reading the data. Constant components are described in NSData.ReadingOptions.

## Return Value

A data object initialized by reading into it the data from the file specified by `path`.

## Discussion

Handling Errors in Swift

In Swift, this API is imported as an initializer and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Reading Data from a File

convenience init?(contentsOfURL: URL)

Creates a data object from the data at the specified file URL.

convenience init(contentsOfURL: URL, options: NSData.ReadingOptions) throws

Creates a data object from the data at the provided file URL using specific reading options.

init?(contentsOfFile: String)

Initializes a data object with the content of the file at a given path.

init?(contentsOfURL: URL)

Creates a data object from the data at the specified file URL, or returns `nil` if the system can’t create one.

init(contentsOfURL: URL, options: NSData.ReadingOptions) throws

Creates a data object from the data at the provided file URL using specific reading options.

struct ReadingOptions

Options for methods used to read data objects.

init?(contentsOfMappedFile: String)

Initializes a data object with the contents of the mapped file specified by a given path.

Deprecated

class func dataWithContentsOfMappedFile(String) -> Any?

Creates a data object from the mapped file at a given path.

Deprecated

