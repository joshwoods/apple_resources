

- Foundation
- NSData
-  init(base64EncodedData:options:) 

Initializer

# init(base64EncodedData:options:)

Initializes a data object with the given Base64 encoded data.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    base64EncodedData base64Data: Data,
    options: NSData.Base64DecodingOptions = []
)
```

``` source
init?(
    base64Encoded base64Data: Data,
    options: NSData.Base64DecodingOptions = []
)
```

## Parameters 

`base64Data`  

A Base64, UTF-8 encoded data object.

`options`  

A mask that specifies options for Base64 decoding the data. Possible values are given in NSData.Base64DecodingOptions.

## Return Value

A data object containing the Base64 decoded data. Returns `nil` if the data object could not be decoded.

## Discussion

The default implementation of this method will reject non-alphabet characters, including line break characters. To support different encodings and ignore non-alphabet characters, specify an `options` value of ignoreUnknownCharacters.

## See Also

### Encoding and Decoding Base64 Representations

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

struct Base64EncodingOptions

Options for methods used to Base64 encode data.

struct Base64DecodingOptions

Options to modify the decoding algorithm used to decode Base64 encoded data.

