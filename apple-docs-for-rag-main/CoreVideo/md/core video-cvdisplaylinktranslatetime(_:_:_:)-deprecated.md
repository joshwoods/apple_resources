

- Core Video
-  CVDisplayLinkTranslateTime(\_:\_:\_:) Deprecated

Function

# CVDisplayLinkTranslateTime(\_:\_:\_:)

Translates the time in the display link’s time base from one representation to another.

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkTranslateTime(
    _ displayLink: CVDisplayLink,
    _ inTime: UnsafePointer,
    _ outTime: UnsafeMutablePointer
) -> CVReturn
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

## Parameters 

`displayLink`  

The display link whose time base should be used to do the translation.

`inTime`  

A pointer to a `CVTimeStamp` structure containing the source time to translate.

`outTime`  

A pointer to a `CVTimeStamp` structure into which the target time is written. Before calling, you must set the version field (currently `0`) to indicate which version of the structure you want. You should also set the `flags` field to specify which representations to translate to.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## Discussion

Note that the display link has to be running for this call to succeed.

## See Also

### Inspecting Display Links

func CVDisplayLinkGetCurrentCGDisplay(CVDisplayLink) -> CGDirectDisplayID

Gets the current display associated with a display link.

Deprecated

func CVDisplayLinkGetCurrentTime(CVDisplayLink, UnsafeMutablePointer&lt;CVTimeStamp>) -> CVReturn

Retrieves the current (“now”) time of a given display link.

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

