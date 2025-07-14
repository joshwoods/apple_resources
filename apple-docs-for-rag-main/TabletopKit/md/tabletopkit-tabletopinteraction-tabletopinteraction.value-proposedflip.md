

- TabletopKit
- TabletopInteraction
- TabletopInteraction.Value
-  proposedFlip 

Instance Property

# proposedFlip

Was the object flipped from the start of this interaction

visionOS 2.0+

``` source
var proposedFlip: Bool { get }
```

## See Also

### Getting the proposed locations

var proposedDestination: TabletopInteraction.Destination?

The proposed destination of the main interaction object, computed from the current pose of the object. During a toss simulation, the proposed destination is only updated if there is only one tossed equipment and it is the currently controlled equipment.

