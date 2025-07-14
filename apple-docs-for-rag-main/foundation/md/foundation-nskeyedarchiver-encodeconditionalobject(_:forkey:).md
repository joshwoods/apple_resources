

- Foundation
- NSKeyedArchiver
-  encodeConditionalObject(\_:forKey:) 

Instance Method

# encodeConditionalObject(\_:forKey:)

Encodes a reference to a given object and associates it with a key only if it has been unconditionally encoded elsewhere in the archive.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func encodeConditionalObject(
    _ object: Any?,
    forKey key: String
)
```

## Parameters 

`object`  

The object to encode.

`key`  

The key with which to associate the encoded value. This value must not be `nil`.

## Discussion

This method is effective only if you’ve previously archived this object with this key by calling encodeInt:forKey:.

## See Also

### Encoding Data and Objects

func encodeEncodable&lt;T>(T, forKey: String) throws

Encodes a given value and associates it with a key.

func encode(Bool, forKey: String)

Encodes a given Boolean value and associates it with a key.

func encodeBytes(UnsafePointer&lt;UInt8>?, length: Int, forKey: String)

Encodes a given number of bytes from a given C array of bytes and associates them with a key.

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

