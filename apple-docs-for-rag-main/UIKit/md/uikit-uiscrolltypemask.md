

- UIKit
-  UIScrollTypeMask 

Structure

# UIScrollTypeMask

A bit mask identifying the scroll type of a pan gesture.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
struct UIScrollTypeMask
```

## Topics

### Scroll types

static var all: UIScrollTypeMask

A scroll type that’s either discrete or continuous.

static var continuous: UIScrollTypeMask

A continuous scroll type from a device, like a trackpad.

static var discrete: UIScrollTypeMask

A discrete scroll type from a device, like a mouse.

### Initializer

init(rawValue: Int)

Creates a new scroll type mask from the raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Tracking scroll events

var allowedScrollTypesMask: UIScrollTypeMask

A scroll type mask that enables recognition of scroll events.

enum UIScrollType

Constants that define the type of the scroll.

