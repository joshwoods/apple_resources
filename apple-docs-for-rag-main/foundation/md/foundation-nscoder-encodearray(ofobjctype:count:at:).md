

- Foundation
- NSCoder
-  encodeArray(ofObjCType:count:at:) 

Instance Method

# encodeArray(ofObjCType:count:at:)

Encodes an array of the given Objective-C type, provided the number of items and a pointer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func encodeArray(
    ofObjCType type: UnsafePointer,
    count: Int,
    at array: UnsafeRawPointer
)
```

## Discussion

The values are encoded from the buffer beginning at `address`. `itemType` must contain exactly one type code. `NSCoder`’s implementation invokes encodeValue(ofObjCType:at:) to encode the entire array of items. Subclasses that implement the encodeValue(ofObjCType:at:) method do not need to override this method.

This method must be matched by a subsequent decodeArray(ofObjCType:count:at:) message.

For information on creating an Objective-C type code suitable for `itemType`, see Type Encodings.

### Special Considerations

You should not use this method to encode C arrays of Objective-C objects. See decodeArray(ofObjCType:count:at:) for more details.

## See Also

### Encoding General Data

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

func encode(Any?)

Encodes an object.

