

- WatchKit
- WKCrownSequencer
-  rotationsPerSecond 

Instance Property

# rotationsPerSecond

The rotational speed of the crown, measured in rotations per second.

watchOS 3.0+

``` source
var rotationsPerSecond: Double { get }
```

## Discussion

This property contains the last reported rotational speed of the crown in rotations per second. The rotational speed is an absolute value. It is always positive, regardless of the rotation’s direction.

## See Also

### Related Documentation

func crownDidRotate(WKCrownSequencer?, rotationalDelta: Double)

Called when the user rotates the crown.

### Getting the Current Crown Status

var isIdle: Bool

A Boolean value indicating whether the crown is at rest.

