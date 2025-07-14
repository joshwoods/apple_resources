

- Swift
- KeyedDecodingContainerProtocol
-  decodeIfPresent(\_:forKey:) 

Instance Method

# decodeIfPresent(\_:forKey:)

Decodes a value of the given type for the given key, if present.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decodeIfPresent(
    _ type: String.Type,
    forKey key: Self.Key
) throws -> String?
```

**Required** Default implementations provided.

## Parameters 

`type`  

The type of value to decode.

`key`  

The key that the decoded value is associated with.

## Return Value

A decoded value of the requested type, or `nil` if the `Decoder` does not have an entry associated with the given key, or if the value is a null value.

## Discussion

This method returns `nil` if the container does not have a value associated with `key`, or if the value is null. The difference between these states can be distinguished with a `contains(_:)` call.

Throws

`DecodingError.typeMismatch` if the encountered encoded value is not convertible to the requested type.

## Default Implementations

### KeyedDecodingContainerProtocol Implementations

func decodeIfPresent(Int8.Type, forKey: Self.Key) throws -> Int8?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(UInt8.Type, forKey: Self.Key) throws -> UInt8?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(UInt128.Type, forKey: Self.Key) throws -> UInt128?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(UInt16.Type, forKey: Self.Key) throws -> UInt16?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Int16.Type, forKey: Self.Key) throws -> Int16?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Int.Type, forKey: Self.Key) throws -> Int?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Int32.Type, forKey: Self.Key) throws -> Int32?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(UInt.Type, forKey: Self.Key) throws -> UInt?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent&lt;T>(T.Type, forKey: Self.Key) throws -> T?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Int128.Type, forKey: Self.Key) throws -> Int128?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(UInt32.Type, forKey: Self.Key) throws -> UInt32?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Float.Type, forKey: Self.Key) throws -> Float?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Bool.Type, forKey: Self.Key) throws -> Bool?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Int64.Type, forKey: Self.Key) throws -> Int64?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(UInt64.Type, forKey: Self.Key) throws -> UInt64?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(String.Type, forKey: Self.Key) throws -> String?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Double.Type, forKey: Self.Key) throws -> Double?

Decodes a value of the given type for the given key, if present.

