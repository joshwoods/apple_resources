

- Foundation
- NSData
-  init(contentsOfMappedFile:) Deprecated

Initializer

# init(contentsOfMappedFile:)

Initializes a data object with the contents of the mapped file specified by a given path.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
init?(contentsOfMappedFile path: String)
```

Deprecated

Use -initWithContentsOfURL:options:error: and NSDataReadingMappedIfSafe or NSDataReadingMappedAlways instead.

## Parameters 

`path`  

The absolute path of the file from which to read data.

## Return Value

A data object initialized by reading into it the mapped file specified by `path`.

## See Also

### Reading Data from a File

convenience init?(contentsOfURL: URL)

Creates a data object from the data at the specified file URL.

convenience init(contentsOfURL: URL, options: NSData.ReadingOptions) throws

Creates a data object from the data at the provided file URL using specific reading options.

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

class func dataWithContentsOfMappedFile(String) -> Any?

Creates a data object from the mapped file at a given path.

Deprecated

