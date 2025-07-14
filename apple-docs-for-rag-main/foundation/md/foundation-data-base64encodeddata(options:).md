

- Foundation
- Data
-  base64EncodedData(options:) 

Instance Method

# base64EncodedData(options:)

Returns Base-64 encoded data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func base64EncodedData(options: Data.Base64EncodingOptions = []) -> Data
```

## Parameters 

`options`  

The options to use for the encoding. Default value is `[]`.

## Return Value

The Base-64 encoded data.

## See Also

### Base-64 Encoding

func base64EncodedString(options: Data.Base64EncodingOptions) -> String

Returns a Base-64 encoded string.

typealias Base64DecodingOptions

Options to use when decoding data.

typealias Base64EncodingOptions

Options to use when encoding data.

