

- Foundation
- NSCoder
-  allowsKeyedCoding 

Instance Property

# allowsKeyedCoding

A Boolean value that indicates whether the receiver supports keyed coding of objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var allowsKeyedCoding: Bool { get }
```

## Discussion

false by default. Concrete subclasses that support keyed coding, such as `NSKeyedArchiver`, need to override this property to return true.

## See Also

### Related Documentation

Archives and Serializations Programming Guide

### Inspecting a Coder

func containsValue(forKey: String) -> Bool

Returns a Boolean value that indicates whether an encoded value is available for a string.

var decodingFailurePolicy: NSCoder.DecodingFailurePolicy

The action the coder should take when decoding fails.

enum DecodingFailurePolicy

Policies describing the action the coder should take when encountering decode failures.

