

- SwiftUI
- View
-  listItemTint(\_:) 

Instance Method

# listItemTint(\_:)

Sets a fixed tint color for content in a list.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func listItemTint(_ tint: Color?) -> some View
```

Show all declarations

## Parameters 

`tint`  

The color to use to tint the content. Use `nil` to avoid overriding the inherited tint.

## Discussion

The containing list’s style applies the tint as appropriate. For example, watchOS uses the tint color for its background platter appearance. Sidebars on iOS and macOS apply the tint color to their Label icons, which otherwise use the accent color by default.

Note

This modifier is equivalent to using the version of the modifier that takes a ListItemTint value and specifying the `tint` color in the corresponding fixed(_:) input.

## See Also

### Configuring rows

func listRowInsets(EdgeInsets?) -> some View

Applies an inset to the rows in a list.

func listRowHoverEffect(HoverEffect?) -> some View

Requests that the containing list row use the provided hover effect.

func listRowHoverEffectDisabled(Bool) -> some View

Requests that the containing list row have its hover effect disabled.

struct ListItemTint

A tint effect configuration that you can apply to content in a list.

var defaultMinListRowHeight: CGFloat

The default minimum height of a row in a `List`. The default minimum height of a row in a list.

