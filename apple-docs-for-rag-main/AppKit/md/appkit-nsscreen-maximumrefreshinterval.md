

- AppKit
- NSScreen
-  maximumRefreshInterval 

Instance Property

# maximumRefreshInterval

The largest refresh interval that the screen supports.

macOS 12.0+

``` source
var maximumRefreshInterval: TimeInterval { get }
```

## Discussion

This interval represents the maximum amount of time (in seconds) your app has to generate new frames. It corresponds to the lowest refresh rate of the display.

## See Also

### Getting Variable Refresh Rate Details

var maximumFramesPerSecond: Int

The maximum number of frames per second that the screen supports.

var minimumRefreshInterval: TimeInterval

The shortest refresh interval that the screen supports.

var displayUpdateGranularity: TimeInterval

The number of seconds between the screen’s supported update rates, for screens that support fixed update rates.

var lastDisplayUpdateTimestamp: TimeInterval

The time of the last framebuffer update, expressed as the number of seconds since system startup.

