

- SwiftUI
- EnvironmentValues
-  defaultMinListRowHeight 

Instance Property

# defaultMinListRowHeight

The default minimum height of a row in a `List`. The default minimum height of a row in a list.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var defaultMinListRowHeight: CGFloat { get set }
```

## See Also

### Configuring rows

func listRowInsets(EdgeInsets?) -> some View

Applies an inset to the rows in a list.

func listRowHoverEffect(HoverEffect?) -> some View

Requests that the containing list row use the provided hover effect.

func listRowHoverEffectDisabled(Bool) -> some View

Requests that the containing list row have its hover effect disabled.

func listItemTint(_:)

Sets a fixed tint color for content in a list.

struct ListItemTint

A tint effect configuration that you can apply to content in a list.

