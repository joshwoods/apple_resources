

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:tintConfigurationForItem:) 

Instance Method

# outlineView(\_:tintConfigurationForItem:)

Customizes an item’s tinting behavior.

macOS 11.0+

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    tintConfigurationForItem item: Any
) -> NSTintConfiguration?
```

## Parameters 

`outlineView`  

The outline view to which you apply the tinting behavior.

`item`  

The item to which you apply the tinting behavior.

## Return Value

Returns a new NSTintConfiguration object to create a particular tinting behavior for the item’s row, or `nil` to inherit the tinting behavior from the item’s parent.

## Discussion

You typically use this method to customize the color for a sidebar.

## See Also

### Customizing Tint Color

class NSTintConfiguration

An object that gives you the ability to choose from system-provided tinting behaviors.

