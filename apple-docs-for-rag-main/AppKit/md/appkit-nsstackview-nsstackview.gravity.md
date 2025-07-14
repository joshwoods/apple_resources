

- AppKit
- NSStackView
-  NSStackView.Gravity 

Enumeration

# NSStackView.Gravity

The gravity areas available in a stack view.

macOS 10.9+

``` source
enum Gravity
```

## Overview

The layout of a stack view is partitioned into three distinct areas in which you can place views. These are known as *gravity areas*. You can use these constants to configure a stack view by way of the insertView(_:at:in:) and setViews(_:in:) methods.

In a horizontally oriented stack view, the three gravity areas are leading, NSStackView.Gravity.center, and trailing. The ordering of these areas depends on the user interface language, unless you’ve explicitly specified the stack view’s user interface layout direction by calling the inherited userInterfaceLayoutDirection method. For a userInterfaceLayoutDirection property value of NSUserInterfaceLayoutDirection.leftToRight, the leading gravity area is on the left.

In a vertically oriented stack view, the three gravity areas are always NSStackView.Gravity.top, NSStackView.Gravity.center, and NSStackView.Gravity.bottom.

The center gravity area is constrained to remain geometrically centered with an Auto Layout priority of defaultLow. For information about geometric spacing between gravity areas, see the description of the spacing property.

## Topics

### Constants

case top

The topmost gravity area in a vertically oriented stack view.

static var leading: NSStackView.Gravity

The leftmost or rightmost gravity area in a horizontally oriented stack view, based on the user interface language or the explicitly set user interface layout direction.

case center

The center gravity area, regardless of stack view layout direction or user interface language.

case bottom

The bottommost gravity area in a vertically oriented stack view.

static var trailing: NSStackView.Gravity

The leftmost or rightmost gravity area in a horizontally oriented stack view, based on the user interface language or the explicitly set user interface layout direction.

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

### Managing Views in Gravity Areas

func addView(NSView, in: NSStackView.Gravity)

Adds a view to the end of the stack view gravity area.

func insertView(NSView, at: Int, in: NSStackView.Gravity)

Adds a view to a stack view gravity area at a specified index position.

func setViews([NSView], in: NSStackView.Gravity)

Specifies an array of views for a specified gravity area in the stack view, replacing any previous views in that area.

func removeView(NSView)

Removes a specified view from the stack view.

