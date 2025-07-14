

- Foundation
- NSKeyedArchiver
-  encode(\_:forKey:) 

Instance Method

# encode(\_:forKey:)

Encodes a given `double` value and associates it with a key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func encode(
    _ value: Double,
    forKey key: String
)
```

## Parameters 

`value`  

The value to encode.

`key`  

The key with which to associate `realv`. This value must not be `nil`.

## See Also

### Related Documentation

func decodeFloat(forKey: String) -> Float

Decodes a single-precision floating-point value associated with a given key.

func decodeDouble(forKey: String) -> Double

Decodes a double-precision floating-point value associated with a given key.

### Encoding Data and Objects

func encodeEncodable&lt;T>(T, forKey: String) throws

Encodes a given value and associates it with a key.

func encode(Bool, forKey: String)

Encodes a given Boolean value and associates it with a key.

func encodeBytes(UnsafePointer&lt;UInt8>?, length: Int, forKey: String)

Encodes a given number of bytes from a given C array of bytes and associates them with a key.

func encodeConditionalObject(Any?, forKey: String)

Encodes a reference to a given object and associates it with a key only if it has been unconditionally encoded elsewhere in the archive.

func encode(Float, forKey: String)

Encodes a given `float` value and associates it with a key.

func encode(Int32, forKey: String)

Encodes a given 32-bit integer value and associates it with a key.

func encode(Int64, forKey: String)

Encodes a given 64-bit integer value and associates it with a key.

func encode(Any?, forKey: String)

Encodes a given object and associates it with a given key.

