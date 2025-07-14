

- UIKit
- UIView
- UIView.Invalidations
-  UIView.Invalidations.Tuple 

Structure

# UIView.Invalidations.Tuple

A change that invalidates a combination of factors covered by the other invalidation types.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOSSwift 5.1+

``` source
struct Tuple where Invalidation1 : UIViewInvalidating, Invalidation2 : UIViewInvalidating
```

## Overview

The system uses this type when a change invalidates multiple aspects of a view. Use a tuple of the static values defined in UIViewInvalidating when more than one invalidation type applies to a change.

## Topics

### Creating the invalidation structure

init(Invalidation1, Invalidation2)

Creates an invalidation structure with multiple invalidations.

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

struct Layout

A change that invalidates the layout of the containing view’s subviews.

