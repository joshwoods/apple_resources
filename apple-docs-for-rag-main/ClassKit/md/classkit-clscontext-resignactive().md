

- ClassKit
- CLSContext
-  resignActive() 

Instance Method

# resignActive()

Tells a context to stop being the active context.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
func resignActive()
```

## Mentioned in 

Informing ClassKit that a task is about to begin

## Discussion

Only one context can be active at a time, so the framework automatically calls this method for you if you activate another context.

## See Also

### Activating and deactivating a context

Informing ClassKit that a task is about to begin

Activate and deactivate contexts according to user interaction.

func becomeActive()

Tells a context to become the active context.

var isActive: Bool

A Boolean indicating whether the context is active.

