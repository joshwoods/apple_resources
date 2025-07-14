

- TabletopKit
- TabletopGame
- TabletopGame.Observer
-  interactionWasUpdated(\_:snapshot:) 

Instance Method

# interactionWasUpdated(\_:snapshot:)

Called whenever any player interaction (local or remote) is updated. Remote player interaction updates always include phase `.started` and `.ended` or `.cancelled` but may not include a phase `.update` for every change to the pose or proposedDestination.

visionOS 2.0+

``` source
func interactionWasUpdated(
    _ value: TabletopInteraction.Value,
    snapshot: TableSnapshot
)
```

**Required** Default implementation provided.

## Default Implementations

### TabletopGame.Observer Implementations

func interactionWasUpdated(TabletopInteraction.Value, snapshot: TableSnapshot)

Called whenever any player interaction (local or remote) is updated. Remote player interaction updates always include phase `.started` and `.ended` or `.cancelled` but may not include a phase `.update` for every change to the pose or proposedDestination.

