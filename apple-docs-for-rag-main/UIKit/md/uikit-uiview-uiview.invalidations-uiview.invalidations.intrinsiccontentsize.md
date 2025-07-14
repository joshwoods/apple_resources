

- UIKit
- UIView
- UIView.Invalidations
-  UIView.Invalidations.IntrinsicContentSize 

Structure

# UIView.Invalidations.IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOSSwift 5.1+

``` source
struct IntrinsicContentSize
```

## Overview

Use intrinsicContentSize to create an instance of this type.

## Topics

### Creating the invalidation structure

var intrinsicContentSize: CGSize

The natural size for the receiving view, considering only properties of the view itself.

init()

Creates an intrinsic content size invalidation structure.

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

struct Layout

A change that invalidates the layout of the containing view’s subviews.

struct Tuple

A change that invalidates a combination of factors covered by the other invalidation types.

