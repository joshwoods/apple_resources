

- UIKit
- UIViewInvalidating
-  constraints 

Type Property

# constraints

A change that invalidates a view’s constraints.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOSSwift 5.1+

``` source
static var constraints: UIView.Invalidations.Constraints { get }
```

Available when `Self` is `UIView.Invalidations.Constraints`.

## Discussion

Use this invalidation type to call setNeedsUpdateConstraints() when a change in property value should cause the containing view to update constraints.

## See Also

### Specifying invalidation types

static var configuration: UIView.Invalidations.Configuration

A change that invalidates a view’s configuration.

static var display: UIView.Invalidations.Display

A change that requires the system to redraw a view’s content.

static var intrinsicContentSize: UIView.Invalidations.IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

static var layout: UIView.Invalidations.Layout

A change that invalidates the layout of the containing view’s subviews.

