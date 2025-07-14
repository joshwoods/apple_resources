

- PHASE
- PHASEEngine
-  init(updateMode:) 

Initializer

# init(updateMode:)

Creates an engine updated by the app or framework.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
init(updateMode: PHASEEngine.UpdateMode)
```

## Parameters 

`updateMode`  

An option that controls the timing of internal framework updates.

## Discussion

The argument you choose determines the rate at which the engine consumes user commands, performs internal updates, and executes callbacks.

When an app calls a PHASE function, the framework defers processing the call until the next update. An engine you configure with PHASEEngine.UpdateMode.manual controls when the framework processes those calls. For example, an app can ensure that two sound events begin simultaneously by following their creation with an update(). Apps that don’t require advanced call synchronization select PHASEEngine.UpdateMode.automatic.

## See Also

### Creating an Engine

enum UpdateMode

Modes that determine when the framework consumes API calls and updates internal state.

