

- Foundation
- NSKeyedUnarchiver
-  decodingFailurePolicy 

Instance Property

# decodingFailurePolicy

The action to take when this unarchiver fails to decode an entry.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var decodingFailurePolicy: NSCoder.DecodingFailurePolicy { get set }
```

## Discussion

The unarchiver may fail to decode an entry for the following reasons:

- The keyed archive data is corrupt or missing.

- A type mismatch occurs, such as expecting a class by calling decodeObject(of:forKey:), but the unarchiver encounters a numeric value for that key instead. This also occurs when decodeIntForKey: encounters a value encoded as floating-point, or vice versa.

- A secure coding violation occurs. This happens when attempting to decode an object that doesn’t conform to NSSecureCoding. This also happens when the encoded type doesn’t match any of the classes passed to unarchivedObject(ofClasses:from:).

## See Also

### Decoding Data

func containsValue(forKey: String) -> Bool

Returns a Boolean value that indicates whether the archive contains a value for a given key within the current decoding scope.

func decodeDecodable&lt;T>(T.Type, forKey: String) -> T?

Decodes a decodable value associated with a given key.

func decodeTopLevelDecodable&lt;T>(T.Type, forKey: String) throws -> T?

Decodes a top-level decodable value associated with a given key.

func decodeBool(forKey: String) -> Bool

Decodes a Boolean value associated with a given key.

func decodeBytes(forKey: String, returnedLength: UnsafeMutablePointer&lt;Int>?) -> UnsafePointer&lt;UInt8>?

Decodes a stream of bytes associated with a given key.

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

