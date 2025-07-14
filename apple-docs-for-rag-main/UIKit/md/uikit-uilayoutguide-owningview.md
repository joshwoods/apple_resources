

- UIKit
- UILayoutGuide
-  owningView 

Instance Property

# owningView

The view that owns this layout guide.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
weak var owningView: UIView? { get set }
```

## Discussion

By default, this property is `nil`. To participate in Auto Layout, the layout guide must be added to a view by calling its addLayoutGuide(_:) method. Do not modify this property directly. Instead, use the view’s addLayoutGuide(_:) and removeLayoutGuide(_:) methods, which update this property as necessary.

## See Also

### Working with layout guides

var identifier: String

A string used to identify the layout guide.

var layoutFrame: CGRect

The layout guide’s frame in its owning view’s coordinate system.

