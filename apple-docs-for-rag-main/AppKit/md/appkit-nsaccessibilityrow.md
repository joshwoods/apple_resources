

- AppKit
-  NSAccessibilityRow 

Protocol

# NSAccessibilityRow

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a row for a table, list, or outline view.

macOS

``` source
protocol NSAccessibilityRow : NSAccessibilityGroup
```

## Overview

You can further enhance the adopting element by implementing any of the information properties or action methods that the NSAccessibilityProtocol protocol declares.

Explicit Implementation Required

Any class that adopts this protocol must implement all of its methods, and the required methods of any protocol it inherits from. The compiler may require you to override some methods that your ancestors have already implemented. Simply follow the compiler’s warnings, and reimplement these methods as necessary.

## Topics

### Supporting Accessibility

func accessibilityDisclosureLevel() -> Int

Returns the indention level for the row.

func accessibilityIndex() -> Int

Returns the index for the row.

**Required**

## Relationships

### Inherits From

- NSAccessibilityElementProtocol
- NSAccessibilityGroup
- NSObjectProtocol

### Conforming Types

- NSTableRowView

## See Also

### Lists

protocol NSAccessibilityTable

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a table view.

protocol NSAccessibilityList

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a list view.

protocol NSAccessibilityOutline

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as an outline view.

