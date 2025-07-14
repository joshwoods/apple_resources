

- UIKit
- UITabBar
-  selectedItem 

Instance Property

# selectedItem

The currently selected item on the tab bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var selectedItem: UITabBarItem? { get set }
```

## Discussion

Use this property to get the currently selected item. If you change the value of this property, the tab bar selects the corresponding item and updates the tab bar’s appearance accordingly. Set the property to `nil` to clear the selection.

When an item is selected, the tab bar displays the image in the tab bar item’s selectedImage property. If the selectedImageTintColor property is set, the tab bar also applies the color in that property to the selected image. To prevent system coloring of an item, provide images using the UIImage.RenderingMode.alwaysOriginal rendering mode.

The default value for this property is `nil`.

## See Also

### Configuring tab bar items

var items: [UITabBarItem]?

The items displayed by the tab bar.

func setItems([UITabBarItem]?, animated: Bool)

Sets the items on the tab bar, optionally animating any changes into position.

