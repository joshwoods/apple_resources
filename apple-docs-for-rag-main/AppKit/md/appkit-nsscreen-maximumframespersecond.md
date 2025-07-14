

- AppKit
- NSScreen
-  maximumFramesPerSecond 

Instance Property

# maximumFramesPerSecond

The maximum number of frames per second that the screen supports.

macOS 12.0+

``` source
var maximumFramesPerSecond: Int { get }
```

## See Also

### Getting Variable Refresh Rate Details

var minimumRefreshInterval: TimeInterval

The shortest refresh interval that the screen supports.

var maximumRefreshInterval: TimeInterval

The largest refresh interval that the screen supports.

var displayUpdateGranularity: TimeInterval

The number of seconds between the screen’s supported update rates, for screens that support fixed update rates.

var lastDisplayUpdateTimestamp: TimeInterval

The time of the last framebuffer update, expressed as the number of seconds since system startup.

