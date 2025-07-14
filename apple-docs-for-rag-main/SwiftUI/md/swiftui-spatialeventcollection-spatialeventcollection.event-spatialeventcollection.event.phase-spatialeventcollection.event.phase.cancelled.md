

- SwiftUI
- SpatialEventCollection
- SpatialEventCollection.Event
- SpatialEventCollection.Event.Phase
-  SpatialEventCollection.Event.Phase.cancelled 

Case

# SpatialEventCollection.Event.Phase.cancelled

The state associated with this phase was canceled and won’t produce any more updates.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+watchOS 11.0+

``` source
case cancelled
```

## See Also

### Getting the phase

case active

The phase is active and the state associated with it is guaranteed to produce at least one more update.

case ended

The state associated with this phase ended normally and won’t produce any more updates.

