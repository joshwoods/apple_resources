

- Game Controller
- GCRacingWheel
-  isSnapshot 

Instance Property

# isSnapshot

A Boolean value that indicates whether the object is a snapshot of a racing wheel.

Mac Catalyst 16.0+macOS 13.0+

``` source
var isSnapshot: Bool { get }
```

## Discussion

If true, the racing wheel is a snapshot at a moment in time of a real device; otherwise, it’s an actual racing wheel.

## See Also

### Creating snapshots

func capture() -> GCRacingWheel

Returns a snapshot of the racing wheel with its current element values.

