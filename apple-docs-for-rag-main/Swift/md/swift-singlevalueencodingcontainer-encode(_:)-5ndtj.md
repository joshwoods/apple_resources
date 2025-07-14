

- Swift
- SingleValueEncodingContainer
-  encode(\_:) 

Instance Method

# encode(\_:)

Encodes a single value of the given type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func encode(_ value: UInt16) throws
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

