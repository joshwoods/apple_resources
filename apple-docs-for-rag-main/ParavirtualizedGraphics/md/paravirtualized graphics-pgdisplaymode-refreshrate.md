

- Paravirtualized Graphics
- PGDisplayMode
-  refreshRate 

Instance Property

# refreshRate

The mode’s refresh rate.

Mac Catalyst 14.0+macOS 11.0+

``` source
var refreshRate: Double { get }
```

## Discussion

Consider supplying only modes that have a refresh rate equal to that of the host environment’s physical display.

## See Also

### Inspecting Mode Properties

var sizeInPixels: PGDisplayCoord_t

The display mode’s dimensions in pixels.

