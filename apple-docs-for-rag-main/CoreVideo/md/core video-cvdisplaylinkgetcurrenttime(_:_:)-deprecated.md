

- Core Video
-  CVDisplayLinkGetCurrentTime(\_:\_:) Deprecated

Function

# CVDisplayLinkGetCurrentTime(\_:\_:)

Retrieves the current (“now”) time of a given display link.

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkGetCurrentTime(
    _ displayLink: CVDisplayLink,
    _ outTime: UnsafeMutablePointer
) -> CVReturn
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

## Parameters 

`displayLink`  

The display link whose current time you want to obtain.

`outTime`  

A pointer to a `CVTimeStamp` structure. Note that you must set the version in the structure (currently 0) before calling to indicate which version of the timestamp structure you want.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## Discussion

You use this call to obtain the timestamp of the frame that is currently being displayed.

## See Also

### Inspecting Display Links

func CVDisplayLinkGetCurrentCGDisplay(CVDisplayLink) -> CGDirectDisplayID

Gets the current display associated with a display link.

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

