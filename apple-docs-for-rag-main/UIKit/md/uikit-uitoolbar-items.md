

- UIKit
- UIToolbar
-  items 

Instance Property

# items

The items displayed on the toolbar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var items: [UIBarButtonItem]? { get set }
```

## Discussion

The items, instances of UIBarButtonItem, that are visible on the toolbar in the order they appear in this array. Any changes to this property aren’t animated. Use the setItems(_:animated:) method to animate changes.

The default value is `nil`.

## See Also

### Configuring toolbar items

func setItems([UIBarButtonItem]?, animated: Bool)

Sets the items on the toolbar by animating the changes.

