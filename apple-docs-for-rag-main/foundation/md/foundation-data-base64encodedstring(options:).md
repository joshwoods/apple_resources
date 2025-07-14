

- Foundation
- Data
-  base64EncodedString(options:) 

Instance Method

# base64EncodedString(options:)

Returns a Base-64 encoded string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func base64EncodedString(options: Data.Base64EncodingOptions = []) -> String
```

## Parameters 

`options`  

The options to use for the encoding. Default value is `[]`.

## Return Value

The Base-64 encoded string.

## See Also

### Base-64 Encoding

func base64EncodedData(options: Data.Base64EncodingOptions) -> Data

Returns Base-64 encoded data.

typealias Base64DecodingOptions

Options to use when decoding data.

typealias Base64EncodingOptions

Options to use when encoding data.

