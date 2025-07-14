

- Foundation
- NSSecureCoding
-  supportsSecureCoding 

Type Property

# supportsSecureCoding

A Boolean value that indicates whether or not the class supports secure coding.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var supportsSecureCoding: Bool { get }
```

**Required**

## Discussion

When you write a class that supports secure coding, ensure that this class property’s getter returns true.

