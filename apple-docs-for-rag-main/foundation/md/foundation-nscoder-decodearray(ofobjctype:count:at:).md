

- Foundation
- NSCoder
-  decodeArray(ofObjCType:count:at:) 

Instance Method

# decodeArray(ofObjCType:count:at:)

Decodes an array of `count` items, whose Objective-C type is given by `itemType`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decodeArray(
    ofObjCType itemType: UnsafePointer,
    count: Int,
    at array: UnsafeMutableRawPointer
)
```

## Discussion

The items are decoded into the buffer beginning at `address`, which must be large enough to contain them all. `itemType` must contain exactly one type code. `NSCoder`’s implementation invokes decodeValue(ofObjCType:at:) to decode the entire array of items.

This method matches an encodeArray(ofObjCType:count:at:) message used during encoding.

For information on creating an Objective-C type code suitable for `itemType`, see Type Encodings.

### Special Considerations

You should not use this method to decode C arrays of Objective-C objects. For historical reasons, returned objects will have an additional ownership reference which you can only relinquish using CFRelease.

## See Also

### Decoding General Data

func decodeBool(forKey: String) -> Bool

Decodes and returns a boolean value that was previously encoded with encode(_:forKey:) and associated with the string `key`.

func decodeBytes(forKey: String, returnedLength: UnsafeMutablePointer&lt;Int>?) -> UnsafePointer&lt;UInt8>?

Decodes a buffer of data that was previously encoded with encodeBytes(_:length:forKey:) and associated with the string `key`.

func decodeBytes(withReturnedLength: UnsafeMutablePointer&lt;Int>) -> UnsafeMutableRawPointer?

Decodes a buffer of data whose types are unspecified.

func decodeData() -> Data?

Decodes and returns an `NSData` object that was previously encoded with encode(_:). Subclasses must override this method.

func decodeDouble(forKey: String) -> Double

Decodes and returns a double value that was previously encoded with either encode(_:forKey:) or encode(_:forKey:) and associated with the string `key`.

func decodeFloat(forKey: String) -> Float

Decodes and returns a float value that was previously encoded with encode(_:forKey:) or encode(_:forKey:) and associated with the string `key`.

func decodeCInt(forKey: String) -> Int32

Decodes and returns an int value that was previously encoded with encodeCInt(_:forKey:), encode(_:forKey:), encode(_:forKey:), or encode(_:forKey:) and associated with the string `key`.

func decodeInteger(forKey: String) -> Int

Decodes and returns an NSInteger value that was previously encoded with encodeCInt(_:forKey:), encode(_:forKey:), encode(_:forKey:), or encode(_:forKey:) and associated with the string `key`.

func decodeInt32(forKey: String) -> Int32

Decodes and returns a 32-bit integer value that was previously encoded with encodeCInt(_:forKey:), encode(_:forKey:), encode(_:forKey:), or encode(_:forKey:) and associated with the string `key`.

func decodeInt64(forKey: String) -> Int64

Decodes and returns a 64-bit integer value that was previously encoded with encodeCInt(_:forKey:), encode(_:forKey:), encode(_:forKey:), or encode(_:forKey:) and associated with the string `key`.

func decodeObject() -> Any?

Decodes and returns an object that was previously encoded with any of the `encode…Object` methods.

func decodeObject(forKey: String) -> Any?

Decodes and returns a previously-encoded object that was previously encoded with encode(_:forKey:) or encodeConditionalObject(_:forKey:) and associated with the string `key`.

func decodePoint() -> NSPoint

Decodes and returns an NSPoint structure that was previously encoded with encode(_:).

func decodePoint(forKey: String) -> NSPoint

Decodes and returns an NSPoint structure that was previously encoded with encode(_:forKey:).

func decodePropertyList() -> Any?

Decodes a property list that was previously encoded with encodePropertyList(_:).

