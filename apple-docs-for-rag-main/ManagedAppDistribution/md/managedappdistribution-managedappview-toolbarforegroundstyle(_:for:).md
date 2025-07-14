

- ManagedAppDistribution
- ManagedAppView
-  toolbarForegroundStyle(\_:for:) 

Instance Method

# toolbarForegroundStyle(\_:for:)

Specifies the preferred foreground style of bars managed by SwiftUI.

ManagedAppDistributionSwiftUIwatchOS 9.0+

``` source
nonisolated
func toolbarForegroundStyle(
    _ style: S,
    for bars: ToolbarPlacement...
) -> some View where S : ShapeStyle
```

## Discussion

This examples shows a view that renders the navigation bar with a blue foreground color.

```
NavigationStack {
    ContentView()
        .navigationTitle("Blue")
        .toolbarForegroundStyle(
            .blue, for: .navigationBar)
}
```

