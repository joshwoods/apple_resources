

- UIKit
-  UIViewInvalidating 

Protocol

# UIViewInvalidating

Implements a type of invalidation that can occur on a view that requires an update.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOSSwift 5.1+

``` source
protocol UIViewInvalidating
```

## Topics

### Specifying invalidation types

static var configuration: UIView.Invalidations.Configuration

A change that invalidates a view’s configuration.

static var constraints: UIView.Invalidations.Constraints

A change that invalidates a view’s constraints.

static var display: UIView.Invalidations.Display

A change that requires the system to redraw a view’s content.

static var intrinsicContentSize: UIView.Invalidations.IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

static var layout: UIView.Invalidations.Layout

A change that invalidates the layout of the containing view’s subviews.

### Invalidating the view

func invalidate(view: UIView)

Indicates to the system that an aspect of a view is invalid and triggers the necessary update.

**Required**

enum Invalidations

Changes that cause an aspect of a view to be invalid and require an update.

## Relationships

### Conforming Types

- UIView.Invalidations.Configuration
- UIView.Invalidations.Constraints
- UIView.Invalidations.Display
- UIView.Invalidations.IntrinsicContentSize
- UIView.Invalidations.Layout
- UIView.Invalidations.Tuple

## See Also

### Updating the view when property values change

struct Invalidating

A property wrapper that notifies the system that a property value change has invalidated an aspect of the containing view.

