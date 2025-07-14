

- UIKit
- UIAccessibilityLocationDescriptor
-  attributedName 

Instance Property

# attributedName

Returns the attributed string representation of the name for the accessibility location descriptor.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var attributedName: NSAttributedString { get }
```

## See Also

### Getting the descriptor information

var name: String

Returns the plaintext string representation of the name for the accessibility location descriptor.

var point: CGPoint

Returns the geometric point of interest for the accessibility location descriptor within its associated view and in the coordinate space of the view.

var view: UIView?

Returns the view associated with the accessibility location descriptor.

