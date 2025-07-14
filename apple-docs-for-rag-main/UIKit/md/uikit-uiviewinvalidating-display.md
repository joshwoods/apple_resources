

- UIKit
- UIViewInvalidating
-  display 

Type Property

# display

A change that requires the system to redraw a view’s content.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOSSwift 5.1+

``` source
static var display: UIView.Invalidations.Display { get }
```

Available when `Self` is `UIView.Invalidations.Display`.

## Discussion

Use this invalidation type to call setNeedsDisplay() when a change in property value should cause the system to redraw the containing view’s content.

## See Also

### Specifying invalidation types

static var configuration: UIView.Invalidations.Configuration

A change that invalidates a view’s configuration.

static var constraints: UIView.Invalidations.Constraints

A change that invalidates a view’s constraints.

static var intrinsicContentSize: UIView.Invalidations.IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

static var layout: UIView.Invalidations.Layout

A change that invalidates the layout of the containing view’s subviews.

