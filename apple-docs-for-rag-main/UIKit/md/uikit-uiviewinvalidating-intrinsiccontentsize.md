

- UIKit
- UIViewInvalidating
-  intrinsicContentSize 

Type Property

# intrinsicContentSize

A change that invalidates a view’s intrinsic size.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOSSwift 5.1+

``` source
static var intrinsicContentSize: UIView.Invalidations.IntrinsicContentSize { get }
```

Available when `Self` is `UIView.Invalidations.IntrinsicContentSize`.

## Discussion

Use this type of invalidation type to call invalidateIntrinsicContentSize() when a change in property value invalidates the containing view’s intrinsic content size. When you use this type, the constraint-based layout system accounts for the change the next time it updates the layout.

## See Also

### Specifying invalidation types

static var configuration: UIView.Invalidations.Configuration

A change that invalidates a view’s configuration.

static var constraints: UIView.Invalidations.Constraints

A change that invalidates a view’s constraints.

static var display: UIView.Invalidations.Display

A change that requires the system to redraw a view’s content.

static var layout: UIView.Invalidations.Layout

A change that invalidates the layout of the containing view’s subviews.

