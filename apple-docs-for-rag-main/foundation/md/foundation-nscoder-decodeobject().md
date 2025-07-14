

- Foundation
- NSCoder
-  decodeObject() 

Instance Method

# decodeObject()

Decodes and returns an object that was previously encoded with any of the `encode…Object` methods.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decodeObject() -> Any?
```

## Discussion

`NSCoder`’s implementation invokes decodeValue(ofObjCType:at:) to decode the object data.

Subclasses may need to override this method if they override any of the corresponding `encode…Object` methods. For example, if an object was encoded conditionally using the encodeConditionalObject(_:) method, this method needs to check whether the object had actually been encoded.

## See Also

### Related Documentation

func encodeByrefObject(Any?)

An encoding method for subclasses to override such that it creates a proxy, rather than a copy, when decoded.

func encodeBycopyObject(Any?)

An encoding method for subclasses to override such that it creates a copy, rather than a proxy, when decoded.

func encode(Any?)

Encodes an object.

### Decoding General Data

func decodeArray(ofObjCType: UnsafePointer&lt;CChar>, count: Int, at: UnsafeMutableRawPointer)

Decodes an array of `count` items, whose Objective-C type is given by `itemType`.

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

func decodeObject(forKey: String) -> Any?

Decodes and returns a previously-encoded object that was previously encoded with encode(_:forKey:) or encodeConditionalObject(_:forKey:) and associated with the string `key`.

func decodePoint() -> NSPoint

Decodes and returns an NSPoint structure that was previously encoded with encode(_:).

func decodePoint(forKey: String) -> NSPoint

Decodes and returns an NSPoint structure that was previously encoded with encode(_:forKey:).

func decodePropertyList() -> Any?

Decodes a property list that was previously encoded with encodePropertyList(_:).

