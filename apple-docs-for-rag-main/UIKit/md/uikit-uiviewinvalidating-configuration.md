

- UIKit
- UIViewInvalidating
-  configuration 

Type Property

# configuration

A change that invalidates a view’s configuration.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOSSwift 5.1+

``` source
static var configuration: UIView.Invalidations.Configuration { get }
```

Available when `Self` is `UIView.Invalidations.Configuration`.

## Discussion

Use this invalidation type to call setNeedsUpdateConfiguration() when a change in property value should cause the containing view to update the configuration.

Note

You only use this invalidation type on UIView subclasses that support a configuration pattern, using setNeedsUpdateConfiguration() and updateConfiguration() pattern. For example, use this type on UIButton, UICollectionViewCell, UITableViewCell, or UITableViewHeaderFooterView. This type has no effect on UIView subclasses that don’t use a configuration pattern.

## See Also

### Specifying invalidation types

static var constraints: UIView.Invalidations.Constraints

A change that invalidates a view’s constraints.

static var display: UIView.Invalidations.Display

A change that requires the system to redraw a view’s content.

static var intrinsicContentSize: UIView.Invalidations.IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

static var layout: UIView.Invalidations.Layout

A change that invalidates the layout of the containing view’s subviews.

