

- UIKit
- UILayoutGuide
-  layoutFrame 

Instance Property

# layoutFrame

The layout guide’s frame in its owning view’s coordinate system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var layoutFrame: CGRect { get }
```

## Discussion

The layout guide defines a rectangular space in its owning view’s coordinate system. This property contains a valid CGRect value by the time its owning view’s layoutSubviews() method is called.

## See Also

### Related Documentation

func layoutSubviews()

Lays out subviews.

### Working with layout guides

var identifier: String

A string used to identify the layout guide.

var owningView: UIView?

The view that owns this layout guide.

