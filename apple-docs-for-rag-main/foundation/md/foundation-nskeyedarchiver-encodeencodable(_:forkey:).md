

- Foundation
- NSKeyedArchiver
-  encodeEncodable(\_:forKey:) 

Instance Method

# encodeEncodable(\_:forKey:)

Encodes a given value and associates it with a key.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@nonobjc
func encodeEncodable(
    _ value: T,
    forKey key: String
) throws where T : Encodable
```

## Parameters 

`value`  

The value to encode.

`key`  

The key with which to associate the encoded value.

## Discussion

If there’s a problem encoding the value you supply, this method throws an error based on the type of problem:

- The value fails to encode, or contains a nested value that fails to encode—this method throws the corresponding error.

- The value can’t be encoded as a property list—this method throws the EncodingError.invalidValue(_:_:) error.

## See Also

### Encoding Data and Objects

func encode(Bool, forKey: String)

Encodes a given Boolean value and associates it with a key.

func encodeBytes(UnsafePointer&lt;UInt8>?, length: Int, forKey: String)

Encodes a given number of bytes from a given C array of bytes and associates them with a key.

func encodeConditionalObject(Any?, forKey: String)

Encodes a reference to a given object and associates it with a key only if it has been unconditionally encoded elsewhere in the archive.

func encode(Double, forKey: String)

Encodes a given `double` value and associates it with a key.

func encode(Float, forKey: String)

Encodes a given `float` value and associates it with a key.

func encode(Int32, forKey: String)

Encodes a given 32-bit integer value and associates it with a key.

func encode(Int64, forKey: String)

Encodes a given 64-bit integer value and associates it with a key.

func encode(Any?, forKey: String)

Encodes a given object and associates it with a given key.

