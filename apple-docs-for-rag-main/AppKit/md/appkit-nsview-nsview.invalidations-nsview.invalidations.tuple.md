

- AppKit
- NSView
- NSView.Invalidations
-  NSView.Invalidations.Tuple 

Structure

# NSView.Invalidations.Tuple

A change that invalidates a combination of factors covered by the other invalidation types.

macOS 12.0+Swift 5.1+

``` source
struct Tuple where Invalidation1 : NSViewInvalidating, Invalidation2 : NSViewInvalidating
```

## Overview

The system uses this type when a change invalidates multiple aspects of a view. Use a tuple of the static values defined in NSViewInvalidating when more than one invalidation type applies to a change.

## Topics

### Creating the invalidation type

init(Invalidation1, Invalidation2)

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

struct Layout

A change that invalidates the layout of the containing view’s subviews.

struct RestorableState

A change that invalidates the restorable state of the view.

