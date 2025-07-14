

- Foundation
- NSData
-  NSData.ReadingOptions 

Structure

# NSData.ReadingOptions

Options for methods used to read data objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct ReadingOptions
```

## Topics

### Initializers

init(rawValue: UInt)

### Constants

static var mappedIfSafe: NSData.ReadingOptions

A hint indicating the file should be mapped into virtual memory, if possible and safe.

static var uncached: NSData.ReadingOptions

A hint indicating the file should not be stored in the file-system caches.

static var alwaysMapped: NSData.ReadingOptions

Hint to map the file in if possible.

static var mappedIfSafe: NSData.ReadingOptions

A hint indicating the file should be mapped into virtual memory, if possible and safe.

static var uncached: NSData.ReadingOptions

A hint indicating the file should not be stored in the file-system caches.

static var alwaysMapped: NSData.ReadingOptions

Hint to map the file in if possible.

### Legacy Constants

static var dataReadingMapped: NSData.ReadingOptions

Deprecated name for mappedIfSafe.

static var mappedRead: NSData.ReadingOptions

Deprecated name for dataReadingMapped.

static var uncachedRead: NSData.ReadingOptions

Deprecated name for uncached.

static var dataReadingMapped: NSData.ReadingOptions

Deprecated name for mappedIfSafe.

static var mappedRead: NSData.ReadingOptions

Deprecated name for dataReadingMapped.

static var uncachedRead: NSData.ReadingOptions

Deprecated name for uncached.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

init?(contentsOfMappedFile: String)

Initializes a data object with the contents of the mapped file specified by a given path.

Deprecated

class func dataWithContentsOfMappedFile(String) -> Any?

Creates a data object from the mapped file at a given path.

Deprecated

