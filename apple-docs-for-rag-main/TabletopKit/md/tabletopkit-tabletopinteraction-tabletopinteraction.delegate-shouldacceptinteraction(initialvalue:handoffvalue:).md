

- TabletopKit
- TabletopInteraction
- TabletopInteraction.Delegate
-  shouldAcceptInteraction(initialValue:handoffValue:) 

Instance Method

# shouldAcceptInteraction(initialValue:handoffValue:)

visionOS 2.2+

``` source
func shouldAcceptInteraction(
    initialValue: TabletopInteraction.Value,
    handoffValue: TabletopInteraction.Value?
) -> TabletopInteraction.NewInteractionIntent
```

**Required** Default implementation provided.

## Default Implementations

### TabletopInteraction.Delegate Implementations

func shouldAcceptInteraction(initialValue: TabletopInteraction.Value, handoffValue: TabletopInteraction.Value?) -> TabletopInteraction.NewInteractionIntent

