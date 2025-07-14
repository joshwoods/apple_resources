

- ClassKit
- CLSContext
-  isActive 

Instance Property

# isActive

A Boolean indicating whether the context is active.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
var isActive: Bool { get }
```

## Discussion

Use the becomeActive() method to activate a context, and the resignActive() method to deactivate it.

## See Also

### Activating and deactivating a context

Informing ClassKit that a task is about to begin

Activate and deactivate contexts according to user interaction.

func becomeActive()

Tells a context to become the active context.

func resignActive()

Tells a context to stop being the active context.

