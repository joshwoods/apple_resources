

- Foundation
- PropertyListEncoder
-  encode(\_:) 

Instance Method

# encode(\_:)

Returns a property list that represents an encoded version of the value you supply.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func encode(_ value: Value) throws -> Data where Value : Encodable
```

## Parameters 

`value`  

The value to encode as a property list.

## Discussion

If there’s a problem encoding the value you supply, this method throws an error based on the type of problem:

- The value fails to encode, or contains a nested value that fails to encode—this method throws the corresponding error.

- The value can’t be encoded as a property list—this method throws the EncodingError.invalidValue(_:_:) error.

## See Also

### Encoding

init()

Creates a new, reusable property list encoder with the default formatting settings.

func encode&lt;T, C>(T, configuration: C.Type) throws -> Data

func encode&lt;T>(T, configuration: T.EncodingConfiguration) throws -> Data

