

- UIKit
- UIAccessibilityLocationDescriptor
-  init(name:point:in:) 

Initializer

# init(name:point:in:)

Initializes a new accessibility location descriptor with a specified point in a view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
convenience init(
    name: String,
    point: CGPoint,
    in view: UIView
)
```

## See Also

### Initializing the descriptor

init(attributedName: NSAttributedString, point: CGPoint, in: UIView)

Initializes a new accessibility location descriptor using an attributed string and a specified point in a view.

convenience init(name: String, view: UIView)

Initializes a new accessibility location descriptor with a specified view’s activation point.

