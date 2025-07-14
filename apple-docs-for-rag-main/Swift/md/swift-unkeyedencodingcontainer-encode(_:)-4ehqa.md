

- Swift
- UnkeyedEncodingContainer
-  encode(\_:) 

Instance Method

# encode(\_:)

Encodes the given value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func encode(_ value: UInt128) throws
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

func encode(Int128) throws

Encodes the given value.

func encode(UInt128) throws

Encodes the given value.

