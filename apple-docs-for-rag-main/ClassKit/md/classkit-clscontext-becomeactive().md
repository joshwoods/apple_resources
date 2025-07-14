

- ClassKit
- CLSContext
-  becomeActive() 

Instance Method

# becomeActive()

Tells a context to become the active context.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
func becomeActive()
```

## Mentioned in 

Informing ClassKit that a task is about to begin

## Discussion

You activate contexts to inform ClassKit which tasks are most recently or commonly visited.

Only one context can be active at a time, so if you tell a context to become active when another already is, the framework automatically deactivates the old one.

## See Also

### Activating and deactivating a context

Informing ClassKit that a task is about to begin

Activate and deactivate contexts according to user interaction.

func resignActive()

Tells a context to stop being the active context.

var isActive: Bool

A Boolean indicating whether the context is active.

