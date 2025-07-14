

- UIKit
- UIView
- UIView.Invalidations
-  UIView.Invalidations.Constraints 

Structure

# UIView.Invalidations.Constraints

A change that invalidates a view’s constraints.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOSSwift 5.1+

``` source
struct Constraints
```

## Overview

Use constraints to create an instance of this type.

## Topics

### Creating the invalidation structure

var constraints: [NSLayoutConstraint]

The constraints held by the view.

init()

Creates a constraints invalidation structure.

## Relationships

### Conforms To

- UIViewInvalidating

## See Also

### Invalidation types

struct Configuration

A change that invalidates a view’s configuration.

struct Display

A change that requires the system to redraw a view’s content.

struct IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

struct Layout

A change that invalidates the layout of the containing view’s subviews.

struct Tuple

A change that invalidates a combination of factors covered by the other invalidation types.

