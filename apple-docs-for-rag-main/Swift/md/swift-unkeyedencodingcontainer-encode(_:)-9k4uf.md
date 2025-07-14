

- Swift
- UnkeyedEncodingContainer
-  encode(\_:) 

Instance Method

# encode(\_:)

Encodes the given value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func encode(_ value: T) throws where T : Encodable
```

**Required** Default implementations provided.

## Parameters 

`value`  

The value to encode.

## Discussion

Throws

`EncodingError.invalidValue` if the given value is invalid in the current context for this format.

## Default Implementations

### UnkeyedEncodingContainer Implementations

func encode(UInt128) throws

Encodes the given value.

func encode(Int128) throws

Encodes the given value.

