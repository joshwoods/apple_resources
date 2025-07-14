

- AppKit
- NSScrollView
-  NSScrollView.Elasticity 

Enumeration

# NSScrollView.Elasticity

These constants determine the elasticity behavior for an axis of the scrollview.

macOS 10.7+

``` source
enum Elasticity
```

## Topics

### Constants

case automatic

Automatically determine whether to allow elasticity on this axis.

case none

Disallow scrolling beyond document bounds on this axis.

case allowed

Allow content to be scrolled past its bounds on this axis in an elastic fashion.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum FindBarPosition

These constants define the position of the find bar in relation to the scroll view.

