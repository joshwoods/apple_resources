

- ScreenCaptureKit
- SCContentFilter
-  init(display:excludingApplications:exceptingWindows:) 

Initializer

# init(display:excludingApplications:exceptingWindows:)

Creates a filter that captures a display, excluding windows of the specified apps.

Mac Catalyst 18.2+macOS 12.3+

``` source
init(
    display: SCDisplay,
    excludingApplications applications: [SCRunningApplication],
    exceptingWindows: [SCWindow]
)
```

## Parameters 

`display`  

A display to capture.

`applications`  

An array of apps to exclude from capture.

`exceptingWindows`  

An array of windows that are exceptions to the previous rules.

## Discussion

The initializer arguments provide a three-stage filter that gives you fine-grained control over the output:

1.  Specify a display to capture. If you don’t specify additional filter criteria, the stream includes all content for a display.

2.  Specify one or more apps with windows to exclude from the output.

3.  Specify one or more windows that are exceptions to the previous rules. If the previous rules include a window, specifying it as an exception excludes it from the output. Likewise, if the previous rules exclude a window, specifying it as an exception includes it in the output.

## See Also

### Creating a filter

init(desktopIndependentWindow: SCWindow)

Creates a filter that captures only the specified window.

init(display: SCDisplay, including: [SCWindow])

Creates a filter that captures only specific windows from a display.

init(display: SCDisplay, excludingWindows: [SCWindow])

Creates a filter that captures the contents of a display, excluding the specified windows.

init(display: SCDisplay, including: [SCRunningApplication], exceptingWindows: [SCWindow])

Creates a filter that captures a display, including only windows of the specified apps.

