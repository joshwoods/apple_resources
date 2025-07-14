

- UIKit
- UITabBar
-  selectionIndicatorImage 

Instance Property

# selectionIndicatorImage

The image to use for the selection indicator.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var selectionIndicatorImage: UIImage? { get set }
```

## Discussion

Use this property to specify a custom selection image. Your image is rendered on top of the tab bar but behind the contents of the tab bar item itself. The default value of this property is `nil`, which causes the tab bar to apply a default highlight to the selected item.

## See Also

### Configuring selection appearance

var unselectedItemTintColor: UIColor?

The tint color to apply to unselected tabs.

var selectedImageTintColor: UIColor?

The tint color applied to the selected tab bar item.

Deprecated

