

- SwiftUI
- ContainerBackgroundPlacement
-  navigation 

Type Property

# navigation

A background placement inside a NavigationStack or NavigationSplitView.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+watchOS 10.0+

``` source
static let navigation: ContainerBackgroundPlacement
```

## Discussion

For translucent backgrounds in a navigation split view, combine this placement with navigationSplitView.

```
NavigationSplitView {
     … sidebar …
    .containerBackground(.thinMaterial, for: .navigation)
    .containerBackground(Color.green, for: .navigationSplitView)
} detail: {
    // … detail …
    .containerBackground(.thickMaterial, for: .navigation)
}
```

## See Also

### Getting placements

static let tabView: ContainerBackgroundPlacement

A background placement inside a TabView.

static let widget: ContainerBackgroundPlacement

The container background placement for a widget.

