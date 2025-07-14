

- AppKit
-  NSAccessibilityGroup 

Protocol

# NSAccessibilityGroup

A role-based protocol that declares the minimum interface necessary to act as a container for other user interface elements.

macOS

``` source
protocol NSAccessibilityGroup : NSAccessibilityElementProtocol
```

## Overview

Visual users often know that sets of controls go together due to their proximity on the screen. However, you must explicitly define these relationships before assistive apps can use them as well. Use this protocol when you want to logically group a collection of accessibility elements. A view that adopts this protocol indicates that an assistive app should treat its content as a group of controls.

You can further enhance the adopting element by implementing any of the information properties or action methods that the NSAccessibilityProtocol protocol declares.

Explicit Implementation Required

Any class that adopts this protocol must implement all of its methods, and the required methods of any protocol it inherits from. The compiler may require you to override some methods that your ancestors have already implemented. Simply follow the compiler’s warnings, and reimplement these methods as necessary.

## Relationships

### Inherits From

- NSAccessibilityElementProtocol
- NSObjectProtocol

### Inherited By

- NSAccessibilityLayoutArea
- NSAccessibilityLayoutItem
- NSAccessibilityList
- NSAccessibilityOutline
- NSAccessibilityProgressIndicator
- NSAccessibilityRow
- NSAccessibilityTable

### Conforming Types

- NSOutlineView
- NSProgressIndicator
- NSTableRowView
- NSTableView

