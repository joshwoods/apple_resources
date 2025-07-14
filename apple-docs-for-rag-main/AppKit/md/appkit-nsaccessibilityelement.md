

- AppKit
-  NSAccessibilityElement 

Class

# NSAccessibilityElement

The basic infrastructure necessary for interacting with an assistive app.

macOS 10.10+

``` source
class NSAccessibilityElement
```

## Overview

Create subclasses of the NSAccessibilityElement class to represent any of your user interface elements that don’t inherit from NSView or from one of the standard AppKit controls. This class represents your user interface element in the accessibility hierarchy and manages the details necessary for working with assistive apps.

To support accessibility features for a custom user interface element:

1.  Create your NSAccessibilityElement subclass by using element(withRole:frame:label:parent:). You can also set these values using setAccessibilityRole(_:), setAccessibilityLabel(_:) and setAccessibilityParent(_:).

2.  Call the parent’s accessibilityAddChildElement(_:) method to add your subclass. You can also add the subclass to its parent’s accessibilityChildren array using setAccessibilityChildren(_:).

3.  In your subclass, call setAccessibilityFrameInParentSpace(_:). This ensures that your control moves with its superview.

4.  In your subclass, adopt a role-specific protocol, customize the role, and post notifications just as you would handle any other accessible control. See Custom Controls.

5.  In your subclass, implement any additional properties and methods you may need to use to further customize your user interface element’s accessibility behavior. See NSAccessibilityProtocol.

## Topics

### Supporting the Accessibility Hierarchy

class func element(withRole: NSAccessibility.Role, frame: NSRect, label: String?, parent: Any?) -> Any

Instantiates and configures a new accessibility element.

func accessibilityAddChildElement(NSAccessibilityElement)

Adds a child to the accessibility element in the accessibility hierarchy.

func accessibilityFrameInParentSpace() -> NSRect

Returns the accessibility element’s frame in its parent’s coordinate system.

func setAccessibilityFrameInParentSpace(NSRect)

Sets the accessibility element’s frame in its parent’s coordinate system.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityProtocol
- NSObjectProtocol

