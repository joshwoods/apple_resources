

- UIKit
- UITabBar
-  selectedImageTintColor Deprecated

Instance Property

# selectedImageTintColor

The tint color applied to the selected tab bar item.

iOS 5.0–8.0DeprecatediPadOS 5.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var selectedImageTintColor: UIColor? { get set }
```

Deprecated

Use the tintColor property instead.

## Discussion

The default value is `nil`, which results in use of the tab bar’s tintColor property.

## See Also

### Configuring selection appearance

var unselectedItemTintColor: UIColor?

The tint color to apply to unselected tabs.

var selectionIndicatorImage: UIImage?

The image to use for the selection indicator.

