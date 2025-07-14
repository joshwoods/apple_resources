

- Foundation
- NSData
-  NSData.Base64EncodingOptions 

Structure

# NSData.Base64EncodingOptions

Options for methods used to Base64 encode data.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Base64EncodingOptions
```

## Topics

### Initializers

init(rawValue: UInt)

### Constants

static var lineLength64Characters: NSData.Base64EncodingOptions

Set the maximum line length to 64 characters, after which a line ending is inserted.

static var lineLength76Characters: NSData.Base64EncodingOptions

Set the maximum line length to 76 characters, after which a line ending is inserted.

static var endLineWithCarriageReturn: NSData.Base64EncodingOptions

When a maximum line length is set, specify that the line ending to insert should include a carriage return.

static var endLineWithLineFeed: NSData.Base64EncodingOptions

When a maximum line length is set, specify that the line ending to insert should include a line feed.

static var lineLength64Characters: NSData.Base64EncodingOptions

Set the maximum line length to 64 characters, after which a line ending is inserted.

static var lineLength76Characters: NSData.Base64EncodingOptions

Set the maximum line length to 76 characters, after which a line ending is inserted.

static var endLineWithCarriageReturn: NSData.Base64EncodingOptions

When a maximum line length is set, specify that the line ending to insert should include a carriage return.

static var endLineWithLineFeed: NSData.Base64EncodingOptions

When a maximum line length is set, specify that the line ending to insert should include a line feed.

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

### Encoding and Decoding Base64 Representations

init?(base64EncodedData: Data, options: NSData.Base64DecodingOptions)

Initializes a data object with the given Base64 encoded data.

init?(base64Encoding: String)

Initializes a data object initialized with the given Base64 encoded string.

Deprecated

init?(base64EncodedString: String, options: NSData.Base64DecodingOptions)

Initializes a data object with the given Base64 encoded string.

func base64EncodedData(options: NSData.Base64EncodingOptions) -> Data

Creates a Base64, UTF-8 encoded data object from the string using the given options.

func base64EncodedString(options: NSData.Base64EncodingOptions) -> String

Creates a Base64 encoded string from the string using the given options.

func base64Encoding() -> String

Initializes a Base64 encoded string from the string.

Deprecated

struct Base64DecodingOptions

Options to modify the decoding algorithm used to decode Base64 encoded data.

