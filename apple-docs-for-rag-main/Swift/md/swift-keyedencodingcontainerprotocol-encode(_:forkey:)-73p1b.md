

- Swift
- KeyedEncodingContainerProtocol
-  encode(\_:forKey:) 

Instance Method

# encode(\_:forKey:)

Encodes the given value for the given key.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func encode(
    _ value: Int128,
    forKey key: Self.Key
) throws
```

**Required** Default implementations provided.

## Parameters 

`value`  

The value to encode.

`key`  

The key to associate the value with.

## Discussion

Throws

`EncodingError.invalidValue` if the given value is invalid in the current context for this format.

## Default Implementations

### KeyedEncodingContainerProtocol Implementations

func encode(Int128, forKey: Self.Key) throws

Encodes the given value for the given key.

func encode(UInt128, forKey: Self.Key) throws

Encodes the given value for the given key.

