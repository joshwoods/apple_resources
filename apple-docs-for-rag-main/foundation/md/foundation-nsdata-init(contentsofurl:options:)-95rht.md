

- Foundation
- NSData
-  init(contentsOfURL:options:) 

Initializer

# init(contentsOfURL:options:)

Creates a data object from the data at the provided file URL using specific reading options.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    contentsOfURL url: URL,
    options readOptionsMask: NSData.ReadingOptions = []
) throws
```

## Parameters 

`url`  

The location on disk of the data to read.

`readOptionsMask`  

The mask specifying the options to use when reading the data. For more information, see NSData.ReadingOptions.

## Return Value

A data object that contains the file’s data, or nil if the system can’t create one.

## Discussion

Important

As this method runs synchronously and blocks the calling thread until it finishes, don’t invoke it from the main thread. Use file coordination or one of the nonblocking file-related APIs instead. For more information, see Improving performance and stability when accessing the file system.

## See Also

### Reading Data from a File

convenience init?(contentsOfURL: URL)

Creates a data object from the data at the specified file URL.

init?(contentsOfFile: String)

Initializes a data object with the content of the file at a given path.

init(contentsOfFile: String, options: NSData.ReadingOptions) throws

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

