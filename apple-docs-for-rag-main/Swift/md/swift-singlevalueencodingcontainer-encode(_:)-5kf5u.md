

- Swift
- SingleValueEncodingContainer
-  encode(\_:) 

Instance Method

# encode(\_:)

Encodes a single value of the given type.

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

Precondition

May not be called after a previous `self.encode(_:)` call.

## Default Implementations

### SingleValueEncodingContainer Implementations

func encode(UInt128) throws

Encodes a single value of the given type.

func encode(Int128) throws

Encodes a single value of the given type.

func encode(Int128) throws

Encodes a single value of the given type.

func encode(UInt128) throws

Encodes a single value of the given type.

