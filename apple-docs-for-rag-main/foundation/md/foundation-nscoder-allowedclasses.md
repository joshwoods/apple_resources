

- Foundation
- NSCoder
-  allowedClasses 

Instance Property

# allowedClasses

The set of coded classes allowed for secure coding.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var allowedClasses: Set? { get }
```

## Discussion

Secure coders check this set of allowed classes before decoding objects, and all objects must implement the NSSecureCoding protocol.

## See Also

### Secure Coding

var requiresSecureCoding: Bool

Indicates whether the archiver requires all archived classes to resist object substitution attacks.

