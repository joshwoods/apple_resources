

- UIKit
- UITabBar
-  tintColor 

Instance Property

# tintColor

The tint color to apply to the tab bar items.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var tintColor: UIColor! { get set }
```

## Discussion

Assigning a value to this property applies the specified color only to the tab bar’s items. Even if you do not specify a color, the tab bar may tint items using the tint color of one of its ancestor views. For information on how tinting colors are applied to views in a view hierarchy, see the description of the tintColor property in UIView.

