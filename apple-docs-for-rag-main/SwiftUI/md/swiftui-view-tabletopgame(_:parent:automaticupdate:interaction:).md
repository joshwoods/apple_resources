

- SwiftUI
- View
-  tabletopGame(\_:parent:automaticUpdate:interaction:) 

Instance Method

# tabletopGame(\_:parent:automaticUpdate:interaction:)

Supplies a closure which returns a new interaction whenever needed.

TabletopKitSwiftUIvisionOS 2.0+

``` source
@MainActor @preconcurrency
func tabletopGame(
    _ game: TabletopGame,
    parent: Entity,
    automaticUpdate: Bool = true,
    interaction make: @escaping (TabletopInteraction.Value) -> any TabletopInteraction.Delegate
) -> some View
```

## See Also

### Creating a tabletop game

func tabletopGame(TabletopGame, parent: Entity, automaticUpdate: Bool) -> some View

Adds a tabletop game to a view.

