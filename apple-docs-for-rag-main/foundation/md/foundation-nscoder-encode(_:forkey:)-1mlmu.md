

- Foundation
- NSCoder
-  encode(\_:forKey:) 

Instance Method

# encode(\_:forKey:)

Encodes an object and associates it with the string key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func encode(
    _ object: Any?,
    forKey key: String
)
```

## Discussion

Subclasses must override this method to identify multiple encodings of `objv` and encode a reference to `objv` instead. For example, `NSKeyedArchiver` detects duplicate objects and encodes a reference to the original object rather than encode the same object twice.

## See Also

### Related Documentation

func decodeObject(forKey: String) -> Any?

Decodes and returns a previously-encoded object that was previously encoded with encode(_:forKey:) or encodeConditionalObject(_:forKey:) and associated with the string `key`.

### Encoding General Data

func encodeArray(ofObjCType: UnsafePointer&lt;CChar>, count: Int, at: UnsafeRawPointer)

Encodes an array of the given Objective-C type, provided the number of items and a pointer.

func encode(Bool, forKey: String)

Encodes a Boolean value and associates it with the string `key`.

func encodeBycopyObject(Any?)

An encoding method for subclasses to override such that it creates a copy, rather than a proxy, when decoded.

func encodeByrefObject(Any?)

An encoding method for subclasses to override such that it creates a proxy, rather than a copy, when decoded.

func encodeBytes(UnsafeRawPointer?, length: Int)

Encodes a buffer of data of an unspecified type.

func encodeBytes(UnsafePointer&lt;UInt8>?, length: Int, forKey: String)

Encodes a buffer of data, given its length and a pointer, and associates it with a string key.

func encodeConditionalObject(Any?)

An encoding method for subclasses to override to conditionally encode an object, preserving common references to it.

func encodeConditionalObject(Any?, forKey: String)

An encoding method for subclasses to override to conditionally encode an object, preserving common references to it, only if it has been unconditionally encoded.

func encode(Data)

Encodes a given data object.

func encode(Double, forKey: String)

Encodes a double-precision floating point value and associates it with the string key.

func encode(Float, forKey: String)

Encodes a floating point value and associates it with the string key.

func encodeCInt(Int32, forKey: String)

Encodes a C integer value and associates it with the string key.

func encode(Int, forKey: String)

Encodes an integer value and associates it with the string key.

func encode(Int32, forKey: String)

Encodes a 32-bit integer value and associates it with the string key.

func encode(Int64, forKey: String)

Encodes a 64-bit integer value and associates it with the string key.

