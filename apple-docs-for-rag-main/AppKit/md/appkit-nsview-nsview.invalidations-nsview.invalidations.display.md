

- AppKit
- NSView
- NSView.Invalidations
-  NSView.Invalidations.Display 

Structure

# NSView.Invalidations.Display

A change that requires the system to redraw a view’s content.

macOS 12.0+Swift 5.1+

``` source
struct Display
```

## Overview

Use display to create an instance of this type.

## Topics

### Creating the invalidation type

func display()

Displays the view and all its subviews if possible, invoking each of the `NSView` methods lockFocus(), draw(_:), and unlockFocus() as necessary.

init()

Creates the invalidation type.

## Relationships

### Conforms To

- NSViewInvalidating

## See Also

### Types of Invalidations

struct Constraints

A change that invalidates a view’s constraints.

struct IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

struct Layout

A change that invalidates the layout of the containing view’s subviews.

struct RestorableState

A change that invalidates the restorable state of the view.

struct Tuple

A change that invalidates a combination of factors covered by the other invalidation types.

