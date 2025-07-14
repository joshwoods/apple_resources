

- Swift
- RawRepresentable
-  encode(to:) 

Instance Method

# encode(to:)

Encodes this value into the given encoder, when the type’s `RawValue` is `UInt128`.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func encode(to encoder: any Encoder) throws
```

Available when `Self` conforms to `Encodable` and `RawValue` is `UInt128`.

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

This function throws an error if any values are invalid for the given encoder’s format.

