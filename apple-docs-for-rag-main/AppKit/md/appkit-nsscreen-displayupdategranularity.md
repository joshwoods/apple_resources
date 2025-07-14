

- AppKit
- NSScreen
-  displayUpdateGranularity 

Instance Property

# displayUpdateGranularity

The number of seconds between the screen’s supported update rates, for screens that support fixed update rates.

macOS 12.0+

``` source
var displayUpdateGranularity: TimeInterval { get }
```

## Discussion

All screen refresh rates fall between the values in the minimumRefreshInterval and maximumRefreshInterval properties. For screens that support fixed update rates, this property contains the amount of time between two successive rates. For example, if a screen supports update rates between 30Hz and 120Hz with an update granularity of 5ms, the screen supports additional refresh rates of approximately 35Hz, 43Hz, 55Hz, and 75Hz.

If the value of this property is `0`, the screen supports any update rate between the minimum and maximum refresh intervals.

## See Also

### Getting Variable Refresh Rate Details

var maximumFramesPerSecond: Int

The maximum number of frames per second that the screen supports.

var minimumRefreshInterval: TimeInterval

The shortest refresh interval that the screen supports.

var maximumRefreshInterval: TimeInterval

The largest refresh interval that the screen supports.

var lastDisplayUpdateTimestamp: TimeInterval

The time of the last framebuffer update, expressed as the number of seconds since system startup.

