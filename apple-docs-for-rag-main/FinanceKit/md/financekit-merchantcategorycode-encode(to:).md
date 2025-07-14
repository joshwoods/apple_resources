

- FinanceKit
- MerchantCategoryCode
-  encode(to:) 

Instance Method

# encode(to:)

Encodes this value into the given encoder, when the type’s `RawValue` is `Int16`.

FinanceKitSwiftiOS 17.0+iPadOS 17.0+

``` source
func encode(to encoder: any Encoder) throws
```

Available when `Self` conforms to `Encodable` and `RawValue` is `Int16`.

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

This function throws an error if any values are invalid for the given encoder’s format.

