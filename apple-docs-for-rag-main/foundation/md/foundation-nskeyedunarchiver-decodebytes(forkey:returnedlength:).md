

- Foundation
- NSKeyedUnarchiver
-  decodeBytes(forKey:returnedLength:) 

Instance Method

# decodeBytes(forKey:returnedLength:)

Decodes a stream of bytes associated with a given key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decodeBytes(
    forKey key: String,
    returnedLength lengthp: UnsafeMutablePointer?
) -> UnsafePointer?
```

## Parameters 

`key`  

A key in the archive within the current decoding scope. `key` must not be `nil`.

`lengthp`  

Upon return, contains the number of bytes returned.

## Return Value

The stream of bytes associated with the key `key`. Returns `NULL` if `key` does not exist.

## Discussion

The returned value is a pointer to a temporary buffer owned by the receiver. The buffer goes away with the unarchiver, not the containing autorelease pool block. You must copy the bytes into your own buffer if you need the data to persist beyond the life of the receiver.

## See Also

### Related Documentation

func encodeBytes(UnsafePointer&lt;UInt8>?, length: Int, forKey: String)

Encodes a given number of bytes from a given C array of bytes and associates them with a key.

### Decoding Data

func containsValue(forKey: String) -> Bool

Returns a Boolean value that indicates whether the archive contains a value for a given key within the current decoding scope.

func decodeDecodable&lt;T>(T.Type, forKey: String) -> T?

Decodes a decodable value associated with a given key.

func decodeTopLevelDecodable&lt;T>(T.Type, forKey: String) throws -> T?

Decodes a top-level decodable value associated with a given key.

func decodeBool(forKey: String) -> Bool

Decodes a Boolean value associated with a given key.

func decodeDouble(forKey: String) -> Double

Decodes a double-precision floating-point value associated with a given key.

func decodeFloat(forKey: String) -> Float

Decodes a single-precision floating-point value associated with a given key.

func decodeInt32(forKey: String) -> Int32

Decodes a 32-bit integer value associated with a given key.

func decodeInt64(forKey: String) -> Int64

Decodes a 64-bit integer value associated with a given key.

func decodeObject(forKey: String) -> Any?

Decodes and returns an object associated with a given key.

func finishDecoding()

Tells the receiver that you are finished decoding objects.

var decodingFailurePolicy: NSCoder.DecodingFailurePolicy

The action to take when this unarchiver fails to decode an entry.

