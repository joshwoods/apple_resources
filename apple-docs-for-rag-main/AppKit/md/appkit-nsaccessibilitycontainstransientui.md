

- AppKit
-  NSAccessibilityContainsTransientUI 

Protocol

# NSAccessibilityContainsTransientUI

A role-based protocol that declares the minimum interface necessary for an accessibility element to support dynamic UI changes.

macOS

``` source
protocol NSAccessibilityContainsTransientUI : NSAccessibilityElementProtocol
```

## Overview

Use this protocol to support accessibility in a UI that changes dynamically—usually in response to mouse-hover events.

Use this protocol in addition to another role-based protocol. See Custom Controls.

Explicit Implementation Required

Any class that adopts this protocol must implement all of its methods, and the required methods of any protocol it inherits from. The compiler may require you to override some methods that your ancestors have already implemented. Simply follow the compiler’s warnings, and reimplement these methods as necessary.

## Topics

### Supporting Accessibility

func accessibilityPerformShowAlternateUI() -> Bool

Displays the accessibility element’s alternative UI.

**Required**

func accessibilityPerformShowDefaultUI() -> Bool

Returns to the accessibility element’s original UI.

**Required**

func isAccessibilityAlternateUIVisible() -> Bool

Returns a Boolean value that determines whether the accessibility element’s alternative UI is currently visible.

**Required**

## Relationships

### Inherits From

- NSAccessibilityElementProtocol
- NSObjectProtocol

