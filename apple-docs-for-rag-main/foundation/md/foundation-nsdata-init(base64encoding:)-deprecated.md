

- Foundation
- NSData
-  init(base64Encoding:) Deprecated

Initializer

# init(base64Encoding:)

Initializes a data object initialized with the given Base64 encoded string.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
init?(base64Encoding base64String: String)
```

Deprecated

You should transition to either init(base64EncodedString:options:) or init(base64EncodedData:options:).

## Parameters 

`base64String`  

A Base-64 encoded string.

## Return Value

A data object built by Base-64 decoding the provided string. Returns `nil` if the data object could not be decoded.

## Discussion

Although this method was only introduced publicly for iOS 7, it has existed since iOS 4; you can use it if your application needs to target an operating system prior to iOS 7. This method behaves like init(base64EncodedString:options:), but ignores all unknown characters.

## See Also

### Encoding and Decoding Base64 Representations

init?(base64EncodedData: Data, options: NSData.Base64DecodingOptions)

Initializes a data object with the given Base64 encoded data.

init?(base64EncodedString: String, options: NSData.Base64DecodingOptions)

Initializes a data object with the given Base64 encoded string.

func base64EncodedData(options: NSData.Base64EncodingOptions) -> Data

Creates a Base64, UTF-8 encoded data object from the string using the given options.

func base64EncodedString(options: NSData.Base64EncodingOptions) -> String

Creates a Base64 encoded string from the string using the given options.

func base64Encoding() -> String

Initializes a Base64 encoded string from the string.

Deprecated

struct Base64EncodingOptions

Options for methods used to Base64 encode data.

struct Base64DecodingOptions

Options to modify the decoding algorithm used to decode Base64 encoded data.

