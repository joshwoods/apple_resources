

- UIKit
- UIView
- UIView.Invalidations
-  UIView.Invalidations.Layout 

Structure

# UIView.Invalidations.Layout

A change that invalidates the layout of the containing view’s subviews.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOSSwift 5.1+

``` source
struct Layout
```

## Overview

Use layout to create an instance of this type.

## Topics

### Creating the invalidation structure

init()

Creates a layout invalidation structure.

## Relationships

### Conforms To

- UIViewInvalidating

## See Also

### Invalidation types

struct Configuration

A change that invalidates a view’s configuration.

struct Constraints

A change that invalidates a view’s constraints.

struct Display

A change that requires the system to redraw a view’s content.

struct IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

struct Tuple

A change that invalidates a combination of factors covered by the other invalidation types.

