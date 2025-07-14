

- UIKit
-  UIAccessibilityLocationDescriptor 

Class

# UIAccessibilityLocationDescriptor

An accessibility descriptor for a specific geometric point of interest within a view, for use by assistive apps.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIAccessibilityLocationDescriptor
```

## Topics

### Initializing the descriptor

init(attributedName: NSAttributedString, point: CGPoint, in: UIView)

Initializes a new accessibility location descriptor using an attributed string and a specified point in a view.

convenience init(name: String, point: CGPoint, in: UIView)

Initializes a new accessibility location descriptor with a specified point in a view.

convenience init(name: String, view: UIView)

Initializes a new accessibility location descriptor with a specified view’s activation point.

### Getting the descriptor information

var name: String

Returns the plaintext string representation of the name for the accessibility location descriptor.

var attributedName: NSAttributedString

Returns the attributed string representation of the name for the accessibility location descriptor.

var point: CGPoint

Returns the geometric point of interest for the accessibility location descriptor within its associated view and in the coordinate space of the view.

var view: UIView?

Returns the view associated with the accessibility location descriptor.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

