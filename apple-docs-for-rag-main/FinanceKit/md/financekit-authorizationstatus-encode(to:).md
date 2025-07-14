

- FinanceKit
- AuthorizationStatus
-  encode(to:) 

Instance Method

# encode(to:)

Encodes this value into the given encoder.

iOS 17.4+iPadOS 17.4+

``` source
func encode(to encoder: any Encoder) throws
```

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

If the value fails to encode anything, `encoder` will encode an empty keyed container in its place.

This function throws an error if any values are invalid for the given encoder’s format.

