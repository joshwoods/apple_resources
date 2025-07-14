

- SpriteKit
- SKNode
-  accessibilityHitTest(\_:) 

Instance Method

# accessibilityHitTest(\_:)

Returns the frontmost user interface element in the element hierarchy.

macOS

``` source
@MainActor
func accessibilityHitTest(_ point: CGPoint) -> Any?
```

## Parameters 

`point`  

Relative to the bottom-left of the screen, in screen points, and guaranteed to lie within the receiver.

## Discussion

Override this method to implement your own, deeper hit testing within a user interface element.

## See Also

### Providing Accessibility

var accessibilityChildren: [Any]?

An array of user interface elements that represent children of this element.

var accessibilityFrame: CGRect

The size of this user interface element, in screen points.

var accessibilityHelp: String?

The help description of this user interface element; for example, the text shown in a tooltip.

var accessibilityLabel: String?

A short description of this user interface element.

var accessibilityParent: AnyObject?

The user interface element that contains this element.

var accessibilityRole: String?

A string value describing the user interface element type; for example, a button.

var accessibilityRoleDescription: String?

A string value describing the user interface element name and type; for example, the Buy button.

var accessibilitySubrole: String?

A string that defines this user interface element’s subrole; for example, a full-screen button.

var isAccessibilityElement: Bool

A toggle you implement to indicate to the system whether this user interface element should be exposed to the user.

var isAccessibilityEnabled: Bool

A toggle you implement to indicate to the system whether this user interface element should respond to user input.

