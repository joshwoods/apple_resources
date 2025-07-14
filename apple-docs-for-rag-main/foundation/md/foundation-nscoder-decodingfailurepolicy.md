

- Foundation
- NSCoder
-  decodingFailurePolicy 

Instance Property

# decodingFailurePolicy

The action the coder should take when decoding fails.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var decodingFailurePolicy: NSCoder.DecodingFailurePolicy { get }
```

## Discussion

A decode call can fail for the following reasons:

- The keyed archive data is corrupt or missing.

- A type mismatch occurs, such as expecting a class by calling decodeObject(of:forKey:) but encountering a numeric type instead. This also occurs when decodeInteger(forKey:) encounters a value encoded as floating-point, or vice versa.

- A secure coding violation occurs. This happens when you attempt to decode an object that doesn’t conform to NSSecureCoding. This also happens when the encoded type doesn’t match any of the types passed to decodeObject(of:forKey:).

## See Also

### Inspecting a Coder

var allowsKeyedCoding: Bool

A Boolean value that indicates whether the receiver supports keyed coding of objects.

func containsValue(forKey: String) -> Bool

Returns a Boolean value that indicates whether an encoded value is available for a string.

enum DecodingFailurePolicy

Policies describing the action the coder should take when encountering decode failures.

