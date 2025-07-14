

- Core Video
-  CVDisplayLinkGetNominalOutputVideoRefreshPeriod(\_:) Deprecated

Function

# CVDisplayLinkGetNominalOutputVideoRefreshPeriod(\_:)

Retrieves the nominal refresh period of a display link.

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkGetNominalOutputVideoRefreshPeriod(_ displayLink: CVDisplayLink) -> CVTime
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

## Parameters 

`displayLink`  

The display link whose refresh period you want to obtain.

## Return Value

A `CVTime` structure that holds the nominal refresh period. This value is indefinite if an invalid display link was specified.

## Discussion

This call allows one to retrieve the device’s ideal refresh period. For example, an NTSC output device might report 1001/60000 to represent the exact NTSC vertical refresh rate.

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

func CVDisplayLinkGetOutputVideoLatency(CVDisplayLink) -> CVTime

Retrieves the nominal latency of a display link.

Deprecated

func CVDisplayLinkIsRunning(CVDisplayLink) -> Bool

Indicates whether a given display link is running.

Deprecated

func CVDisplayLinkGetTypeID() -> CFTypeID

Obtains the Core Foundation ID for the display link data type.

Deprecated

