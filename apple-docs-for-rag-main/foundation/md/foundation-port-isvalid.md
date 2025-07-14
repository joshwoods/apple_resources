

- Foundation
- Port
-  isValid 

Instance Property

# isValid

A Boolean value that indicates whether the receiver is valid.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isValid: Bool { get }
```

## Discussion

false if the receiver is known to be invalid, otherwise true.

An `NSPort` object becomes invalid when its underlying communication resource, which is operating system dependent, is closed or damaged.

## See Also

### Validation

func invalidate()

Marks the receiver as invalid and posts an didBecomeInvalidNotification to the default notification center.

