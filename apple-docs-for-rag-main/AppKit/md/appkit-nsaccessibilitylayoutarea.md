

- AppKit
-  NSAccessibilityLayoutArea 

Protocol

# NSAccessibilityLayoutArea

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a layout area.

macOS

``` source
protocol NSAccessibilityLayoutArea : NSAccessibilityGroup
```

## Overview

Use this protocol when you want to create a canvas that contains layout items.

You can further enhance the adopting element by implementing any of the information properties or action methods that the NSAccessibilityProtocol protocol declares.

Explicit Implementation Required

Any class that adopts this protocol must implement all of its methods, and the required methods of any protocol it inherits from. The compiler may require you to override some methods that your ancestors have already implemented. Simply follow the compiler’s warnings, and reimplement these methods as necessary.

## Topics

### Supporting Accessibility

func accessibilityChildren() -> [Any]?

Returns the accessibility element’s children in the accessibility hierarchy.

**Required**

var accessibilityFocusedUIElement: Any

The child accessibility element with the current focus.

**Required**

func accessibilityLabel() -> String

Returns a short description of the layout area.

**Required**

func accessibilitySelectedChildren() -> [Any]?

Returns the layout area’s currently selected children.

**Required**

## Relationships

### Inherits From

- NSAccessibilityElementProtocol
- NSAccessibilityGroup
- NSObjectProtocol

## See Also

### Layout Elements

protocol NSAccessibilityLayoutItem

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a layout item.

