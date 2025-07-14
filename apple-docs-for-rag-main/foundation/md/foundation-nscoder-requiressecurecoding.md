

- Foundation
- NSCoder
-  requiresSecureCoding 

Instance Property

# requiresSecureCoding

Indicates whether the archiver requires all archived classes to resist object substitution attacks.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var requiresSecureCoding: Bool { get }
```

## Discussion

true if this coder requires secure coding; false otherwise.

Secure coders check a set of allowed classes before decoding objects, and all objects must implement the NSSecureCoding protocol.

## See Also

### Related Documentation

var allowsKeyedCoding: Bool

A Boolean value that indicates whether the receiver supports keyed coding of objects.

### Secure Coding

var allowedClasses: Set&lt;AnyHashable>?

The set of coded classes allowed for secure coding.

