

- WatchKit
- WKCrownSequencer
-  isIdle 

Instance Property

# isIdle

A Boolean value indicating whether the crown is at rest.

watchOS 3.0+

``` source
var isIdle: Bool { get }
```

## Discussion

The value of this property is true when the user is not rotating the crown and false when the user is rotating the crown.

## See Also

### Related Documentation

func crownDidBecomeIdle(WKCrownSequencer?)

Called when the user stops rotating the crown.

### Getting the Current Crown Status

var rotationsPerSecond: Double

The rotational speed of the crown, measured in rotations per second.

