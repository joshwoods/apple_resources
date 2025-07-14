

- Swift
- RawRepresentable
-  encode(to:) 

Instance Method

# encode(to:)

Encodes this value into the given encoder, when the type’s `RawValue` is `UInt`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func encode(to encoder: any Encoder) throws
```

Available when `Self` conforms to `Encodable` and `RawValue` is `UInt`.

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

This function throws an error if any values are invalid for the given encoder’s format.

## See Also

### Encoding a Value

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `String`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Bool`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Double`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Float`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int8`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int16`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int32`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int64`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `UInt8`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `UInt16`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `UInt32`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `UInt64`.

