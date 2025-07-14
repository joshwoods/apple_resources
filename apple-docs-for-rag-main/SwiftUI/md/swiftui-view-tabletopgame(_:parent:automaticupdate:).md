

- SwiftUI
- View
-  tabletopGame(\_:parent:automaticUpdate:) 

Instance Method

# tabletopGame(\_:parent:automaticUpdate:)

Adds a tabletop game to a view.

TabletopKitSwiftUIvisionOS 2.0+

``` source
@MainActor @preconcurrency
func tabletopGame(
    _ game: TabletopGame,
    parent: Entity,
    automaticUpdate: Bool = true
) -> some View
```

## See Also

### Creating a tabletop game

func tabletopGame(TabletopGame, parent: Entity, automaticUpdate: Bool, interaction: (TabletopInteraction.Value) -> any TabletopInteraction.Delegate) -> some View

Supplies a closure which returns a new interaction whenever needed.

