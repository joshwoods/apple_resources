

- UIKit
- UIToolbar
-  setItems(\_:animated:) 

Instance Method

# setItems(\_:animated:)

Sets the items on the toolbar by animating the changes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setItems(
    _ items: [UIBarButtonItem]?,
    animated: Bool
)
```

## Parameters 

`items`  

The items to display on the toolbar.

`animated`  

A Boolean value if set to true animates the transition to the items; otherwise, does not.

## Discussion

If `animated` is true, the changes are dissolved or the reordering is animated—for example, removed items fade out and new items fade in. This method also adjusts the spacing between items.

## See Also

### Configuring toolbar items

var items: [UIBarButtonItem]?

The items displayed on the toolbar.

