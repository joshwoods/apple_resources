

- AppKit
- NSScreen
-  lastDisplayUpdateTimestamp 

Instance Property

# lastDisplayUpdateTimestamp

The time of the last framebuffer update, expressed as the number of seconds since system startup.

macOS 12.0+

``` source
var lastDisplayUpdateTimestamp: TimeInterval { get }
```

## Discussion

Use this property to determine how much time elapsed since the last frame update.

## See Also

### Getting Variable Refresh Rate Details

var maximumFramesPerSecond: Int

The maximum number of frames per second that the screen supports.

var minimumRefreshInterval: TimeInterval

The shortest refresh interval that the screen supports.

var maximumRefreshInterval: TimeInterval

The largest refresh interval that the screen supports.

var displayUpdateGranularity: TimeInterval

The number of seconds between the screen’s supported update rates, for screens that support fixed update rates.

