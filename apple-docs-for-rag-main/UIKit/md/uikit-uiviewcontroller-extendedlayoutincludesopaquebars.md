

- UIKit
- UIViewController
-  extendedLayoutIncludesOpaqueBars 

Instance Property

# extendedLayoutIncludesOpaqueBars

A Boolean value indicating whether or not the extended layout includes opaque bars.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var extendedLayoutIncludesOpaqueBars: Bool { get set }
```

## Discussion

The default value of this property is false.

Note

Bars are translucent by default in iOS 7.0

## See Also

### Configuring the view’s layout behavior

var edgesForExtendedLayout: UIRectEdge

The edges that you extend for your view controller.

struct UIRectEdge

Constants that specify the edges of a rectangle.

func viewWillLayoutSubviews()

Notifies the view controller that its view is about to lay out its subviews.

func viewDidLayoutSubviews()

Notifies the view controller when its view finishes laying out its subviews.

func updateViewConstraints()

Notifies the view controller when its view needs to update its constraints.

