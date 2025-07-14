

- Core Graphics
- CGEventMouseSubtype
-  CGEventMouseSubtype.defaultType 

Case

# CGEventMouseSubtype.defaultType

Specifies that the event is an ordinary mouse event, and does not contain additional tablet device information.

Mac CatalystmacOS

``` source
case defaultType
```

## See Also

### Constants

case tabletPoint

Specifies that the mouse event originated from a tablet device, and that the various `kCGTabletEvent` field selectors may be used to obtain tablet-specific data from the mouse event.

case tabletProximity

