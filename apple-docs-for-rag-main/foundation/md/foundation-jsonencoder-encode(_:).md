

- Foundation
- JSONEncoder
-  encode(\_:) 

Instance Method

# encode(\_:)

Returns a JSON-encoded representation of the value you supply.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func encode(_ value: T) throws -> Data where T : Encodable
```

## Parameters 

`value`  

The value to encode as JSON.

## Return Value

The encoded JSON data.

## Discussion

If there’s a problem encoding the value you supply, this method throws an error based on the type of problem:

- The value fails to encode, or contains a nested value that fails to encode—this method throws the corresponding error.

- The value isn’t encodable as a JSON array or JSON object—this method throws the EncodingError.invalidValue(_:_:) error.

- The value contains an exceptional floating-point number (such as infinity or nan) and you’re using the default JSONEncoder.NonConformingFloatEncodingStrategy — this method throws the EncodingError.invalidValue(_:_:) error.

## See Also

### First Steps

init()

Creates a new, reusable JSON encoder with the default formatting settings and encoding strategies.

