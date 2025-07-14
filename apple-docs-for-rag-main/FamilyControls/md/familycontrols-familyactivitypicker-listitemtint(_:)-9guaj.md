

- FamilyControls
- FamilyActivityPicker
-  listItemTint(\_:) 

Instance Method

# listItemTint(\_:)

Sets the tint effect for content in a list.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func listItemTint(_ tint: ListItemTint?) -> some View
```

## Parameters 

`tint`  

The tint effect to use. Use `nil` to avoid overriding the inherited tint.

## Discussion

The containing list’s style applies the tint as appropriate. For example, watchOS uses the tint color for its background platter appearance. Sidebars on iOS and macOS apply the tint color to their `Label` icons, which otherwise use the accent color by default.

## See Also

### Tint Color

func tint(Color?) -> some View

Sets the tint color within this view.

func listRowSeparatorTint(Color?, edges: VerticalEdge.Set) -> some View

Sets the tint color associated with a row.

func listSectionSeparatorTint(Color?, edges: VerticalEdge.Set) -> some View

Sets the tint color associated with a section.

func listItemTint(Color?) -> some View

Sets a fixed tint color for content in a list.

