

- AppKit
- NSView
- NSView.Invalidations
-  NSView.Invalidations.IntrinsicContentSize 

Structure

# NSView.Invalidations.IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

macOS 12.0+Swift 5.1+

``` source
struct IntrinsicContentSize
```

## Overview

Use intrinsicContentSize to create an instance of this type.

## Topics

### Creating the invalidation type

var intrinsicContentSize: NSSize

The natural size for the receiving view, considering only properties of the view itself.

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

struct Layout

A change that invalidates the layout of the containing view’s subviews.

struct RestorableState

A change that invalidates the restorable state of the view.

struct Tuple

A change that invalidates a combination of factors covered by the other invalidation types.

