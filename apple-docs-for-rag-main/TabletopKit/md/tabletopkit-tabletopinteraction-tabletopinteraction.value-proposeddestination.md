

- TabletopKit
- TabletopInteraction
- TabletopInteraction.Value
-  proposedDestination 

Instance Property

# proposedDestination

The proposed destination of the main interaction object, computed from the current pose of the object. During a toss simulation, the proposed destination is only updated if there is only one tossed equipment and it is the currently controlled equipment.

visionOS 2.0+

``` source
var proposedDestination: TabletopInteraction.Destination? { get }
```

## See Also

### Getting the proposed locations

var proposedFlip: Bool

Was the object flipped from the start of this interaction

