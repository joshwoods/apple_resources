

- DockKit
- DockAccessory
-  trackingStates 

Instance Property

# trackingStates

Provides an access to the asynchronous sequence of tracking session states

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
final var trackingStates: DockAccessory.TrackingStates { get throws }
```

## Return Value

A `DockAccessory.TrackingStates` instance representing the current state of tracking.

## Discussion

Throws

DockKitError.notConnected if device is disconnected, or DockKitError.notSupportedByDevice if device doesn’t support updates.

