

- Foundation
- NSData
-  dataWithContentsOfMappedFile(\_:) Deprecated

Type Method

# dataWithContentsOfMappedFile(\_:)

Creates a data object from the mapped file at a given path.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
class func dataWithContentsOfMappedFile(_ path: String) -> Any?
```

Deprecated

Use +dataWithContentsOfURL:options:error: and NSDataReadingMappedIfSafe or NSDataReadingMappedAlways instead.

## Parameters 

`path`  

The absolute path of the file from which to read data.

## Discussion

This method returns `nil` if the data object could not be created

Because of file mapping restrictions, this method should only be used if the file is guaranteed to exist for the duration of the data object’s existence. It is generally safer to use the dataWithContentsOfFile: method.

This methods assumes mapped files are available from the underlying operating system. A mapped file uses virtual memory techniques to avoid copying pages of the file into memory until they are actually needed.

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

init?(contentsOfMappedFile: String)

Initializes a data object with the contents of the mapped file specified by a given path.

Deprecated

