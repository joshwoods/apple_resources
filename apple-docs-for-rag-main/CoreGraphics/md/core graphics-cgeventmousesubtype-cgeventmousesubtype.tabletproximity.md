

- Core Graphics
- CGEventMouseSubtype
-  CGEventMouseSubtype.tabletProximity 

Case

# CGEventMouseSubtype.tabletProximity

Mac CatalystmacOS

``` source
case tabletProximity
```

## Discussion

Specifies that the mouse event originated from a tablet device with the pen in proximity but not necessarily touching the tablet, and that the various `kCGTabletProximity` field selectors may be used to obtain tablet-specific data from the mouse event. This is often used with mouse move events originating from a tablet.

## See Also

### Constants

case defaultType

Specifies that the event is an ordinary mouse event, and does not contain additional tablet device information.

case tabletPoint

Specifies that the mouse event originated from a tablet device, and that the various `kCGTabletEvent` field selectors may be used to obtain tablet-specific data from the mouse event.

