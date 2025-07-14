

- UIKit
- UIView
- UIView.Invalidations
-  UIView.Invalidations.Configuration 

Structure

# UIView.Invalidations.Configuration

A change that invalidates a view’s configuration.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOSSwift 5.1+

``` source
struct Configuration
```

## Overview

Use configuration to create an instance of this type.

## Topics

### Creating the invalidation structure

init()

Creates a configuration invalidation structure.

## Relationships

### Conforms To

- UIViewInvalidating

## See Also

### Invalidation types

struct Constraints

A change that invalidates a view’s constraints.

struct Display

A change that requires the system to redraw a view’s content.

struct IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

struct Layout

A change that invalidates the layout of the containing view’s subviews.

struct Tuple

A change that invalidates a combination of factors covered by the other invalidation types.

