

- Core Video
-  CVDisplayLinkGetOutputVideoLatency(\_:) Deprecated

Function

# CVDisplayLinkGetOutputVideoLatency(\_:)

Retrieves the nominal latency of a display link.

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkGetOutputVideoLatency(_ displayLink: CVDisplayLink) -> CVTime
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

## Parameters 

`displayLink`  

The display link whose latency value you want to obtain.

## Return Value

A `CVTime` structure that holds the latency value. This value may be indefinite.

## Discussion

This call allows you to retrieve the device’s built-in output latency. For example, an NTSC device with one frame of latency might report back 1001/30000 or 2002/60000.

## See Also

### Inspecting Display Links

func CVDisplayLinkGetCurrentCGDisplay(CVDisplayLink) -> CGDirectDisplayID

Gets the current display associated with a display link.

Deprecated

func CVDisplayLinkGetCurrentTime(CVDisplayLink, UnsafeMutablePointer&lt;CVTimeStamp>) -> CVReturn

Retrieves the current (“now”) time of a given display link.

Deprecated

func CVDisplayLinkTranslateTime(CVDisplayLink, UnsafePointer&lt;CVTimeStamp>, UnsafeMutablePointer&lt;CVTimeStamp>) -> CVReturn

Translates the time in the display link’s time base from one representation to another.

Deprecated

func CVDisplayLinkGetActualOutputVideoRefreshPeriod(CVDisplayLink) -> Double

Retrieves the actual output refresh period of a display as measured by the system time.

Deprecated

func CVDisplayLinkGetNominalOutputVideoRefreshPeriod(CVDisplayLink) -> CVTime

Retrieves the nominal refresh period of a display link.

Deprecated

func CVDisplayLinkIsRunning(CVDisplayLink) -> Bool

Indicates whether a given display link is running.

Deprecated

func CVDisplayLinkGetTypeID() -> CFTypeID

Obtains the Core Foundation ID for the display link data type.

Deprecated

