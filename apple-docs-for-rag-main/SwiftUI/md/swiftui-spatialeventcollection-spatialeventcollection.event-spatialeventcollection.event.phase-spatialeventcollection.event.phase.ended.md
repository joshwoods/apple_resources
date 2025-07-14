

- SwiftUI
- SpatialEventCollection
- SpatialEventCollection.Event
- SpatialEventCollection.Event.Phase
-  SpatialEventCollection.Event.Phase.ended 

Case

# SpatialEventCollection.Event.Phase.ended

The state associated with this phase ended normally and won’t produce any more updates.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+watchOS 11.0+

``` source
case ended
```

## See Also

### Getting the phase

case active

The phase is active and the state associated with it is guaranteed to produce at least one more update.

case cancelled

The state associated with this phase was canceled and won’t produce any more updates.

