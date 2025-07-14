

- UIKit
- UIView
- UIView.Invalidations
-  UIView.Invalidations.Display 

Structure

# UIView.Invalidations.Display

A change that requires the system to redraw a view’s content.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOSSwift 5.1+

``` source
struct Display
```

## Overview

Use display to create an instance of this type.

## Topics

### Creating the invalidation structure

init()

Creates a display invalidation structure.

## Relationships

### Conforms To

- UIViewInvalidating

## See Also

### Invalidation types

struct Configuration

A change that invalidates a view’s configuration.

struct Constraints

A change that invalidates a view’s constraints.

struct IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

struct Layout

A change that invalidates the layout of the containing view’s subviews.

struct Tuple

A change that invalidates a combination of factors covered by the other invalidation types.

