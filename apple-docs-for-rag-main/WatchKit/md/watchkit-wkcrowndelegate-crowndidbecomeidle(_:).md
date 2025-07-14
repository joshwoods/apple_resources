

- WatchKit
- WKCrownDelegate
-  crownDidBecomeIdle(\_:) 

Instance Method

# crownDidBecomeIdle(\_:)

Called when the user stops rotating the crown.

watchOS 3.0+

``` source
optional func crownDidBecomeIdle(_ crownSequencer: WKCrownSequencer?)
```

## Parameters 

`crownSequencer`  

The crown sequencer object reporting the change.

## Discussion

The crown sequencer calls this method when the crown finally comes to rest. The sequencer calls this method only after one or more calls to the crownDidRotate(_:rotationalDelta:) method.

## See Also

### Related Documentation

var isIdle: Bool

A Boolean value indicating whether the crown is at rest.

### Receiving Crown Events

func crownDidRotate(WKCrownSequencer?, rotationalDelta: Double)

Called when the user rotates the crown.

