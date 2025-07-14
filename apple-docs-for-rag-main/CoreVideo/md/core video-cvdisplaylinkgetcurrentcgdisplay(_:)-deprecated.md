

- Core Video
-  CVDisplayLinkGetCurrentCGDisplay(\_:) Deprecated

Function

# CVDisplayLinkGetCurrentCGDisplay(\_:)

Gets the current display associated with a display link.

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkGetCurrentCGDisplay(_ displayLink: CVDisplayLink) -> CGDirectDisplayID
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

## Parameters 

`displayLink`  

The display link whose current display you want to obtain.

## Return Value

An identifier representing the current display. For more information on the display identifier type, see CGDirectDisplayID.

## See Also

### Inspecting Display Links

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

func CVDisplayLinkGetOutputVideoLatency(CVDisplayLink) -> CVTime

Retrieves the nominal latency of a display link.

Deprecated

func CVDisplayLinkIsRunning(CVDisplayLink) -> Bool

Indicates whether a given display link is running.

Deprecated

func CVDisplayLinkGetTypeID() -> CFTypeID

Obtains the Core Foundation ID for the display link data type.

Deprecated

