

- AppKit
- NSView
- NSView.Invalidations
-  NSView.Invalidations.Layout 

Structure

# NSView.Invalidations.Layout

A change that invalidates the layout of the containing view’s subviews.

macOS 12.0+Swift 5.1+

``` source
struct Layout
```

## Overview

Use layout to create an instance of this type.

## Topics

### Creating the invalidation type

func layout()

Perform layout in concert with the constraint-based layout system.

init()

Creates the invalidation type.

## Relationships

### Conforms To

- NSViewInvalidating

## See Also

### Types of Invalidations

struct Constraints

A change that invalidates a view’s constraints.

struct Display

A change that requires the system to redraw a view’s content.

struct IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

struct RestorableState

A change that invalidates the restorable state of the view.

struct Tuple

A change that invalidates a combination of factors covered by the other invalidation types.

