

- UIKit
-  UIScrollType 

Enumeration

# UIScrollType

Constants that define the type of the scroll.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
enum UIScrollType
```

## Topics

### Constants

case discrete

A discrete scroll type that originates from a device like a mouse with a scroll wheel.

case continuous

A continuous scroll type that originates from a device like a trackpad.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Tracking scroll events

var allowedScrollTypesMask: UIScrollTypeMask

A scroll type mask that enables recognition of scroll events.

struct UIScrollTypeMask

A bit mask identifying the scroll type of a pan gesture.

