

- SwiftUI
- View
-  listRowHoverEffect(\_:) 

Instance Method

# listRowHoverEffect(\_:)

Requests that the containing list row use the provided hover effect.

visionOS 1.0+

``` source
nonisolated
func listRowHoverEffect(_ effect: HoverEffect?) -> some View
```

## Parameters 

`effect`  

The hover effect applied to the entire list row.

## Return Value

A view that requests a hover effect for a containing list row

## Discussion

By default, `List` rows have built-in hover effects in visionOS. In some cases, it is useful to change the default hover effect.

This modifier can be applied to a list row’s content to request that the list row’s default effect be replaced by the provided effect. If the view is not contained within a `List` or if the view does not support hover effects in this context, the modifier has no effect.

Use a `nil` effect to indicate that the list row’s default hover effect should not be modified.

lift is not supported for list rows.

## See Also

### Configuring rows

func listRowInsets(EdgeInsets?) -> some View

Applies an inset to the rows in a list.

func listRowHoverEffectDisabled(Bool) -> some View

Requests that the containing list row have its hover effect disabled.

func listItemTint(_:)

Sets a fixed tint color for content in a list.

struct ListItemTint

A tint effect configuration that you can apply to content in a list.

var defaultMinListRowHeight: CGFloat

The default minimum height of a row in a `List`. The default minimum height of a row in a list.

