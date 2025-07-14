

- AppKit
- NSView
- NSView.Invalidations
-  NSView.Invalidations.Constraints 

Structure

# NSView.Invalidations.Constraints

A change that invalidates a view’s constraints.

macOS 12.0+Swift 5.1+

``` source
struct Constraints
```

## Overview

Use constraints to create an instance of this type.

## Topics

### Creating the invalidation type

var constraints: [NSLayoutConstraint]

Returns the constraints held by the view.

init()

Creates the invalidation type.

## Relationships

### Conforms To

- NSViewInvalidating

## See Also

### Types of Invalidations

struct Display

A change that requires the system to redraw a view’s content.

struct IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

struct Layout

A change that invalidates the layout of the containing view’s subviews.

struct RestorableState

A change that invalidates the restorable state of the view.

struct Tuple

A change that invalidates a combination of factors covered by the other invalidation types.

