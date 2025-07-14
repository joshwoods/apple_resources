

- Swift
- KeyedEncodingContainerProtocol
-  encodeIfPresent(\_:forKey:) 

Instance Method

# encodeIfPresent(\_:forKey:)

Encodes the given value for the given key if it is not `nil`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func encodeIfPresent(
    _ value: UInt?,
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

func encodeIfPresent(UInt?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(String?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int16?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int64?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Double?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt32?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt128?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent&lt;T>(T?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt64?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int8?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Float?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt8?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt16?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Bool?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int128?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int32?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

