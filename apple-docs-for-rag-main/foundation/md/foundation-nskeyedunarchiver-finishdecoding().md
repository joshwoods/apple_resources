

- Foundation
- NSKeyedUnarchiver
-  finishDecoding() 

Instance Method

# finishDecoding()

Tells the receiver that you are finished decoding objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func finishDecoding()
```

## Discussion

Invoking this method allows the receiver to notify its delegate and to perform any final operations on the archive. Once this method is invoked, the receiver cannot decode any further values.

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

var decodingFailurePolicy: NSCoder.DecodingFailurePolicy

The action to take when this unarchiver fails to decode an entry.

