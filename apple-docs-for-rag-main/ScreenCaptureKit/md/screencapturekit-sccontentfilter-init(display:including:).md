

- ScreenCaptureKit
- SCContentFilter
-  init(display:including:) 

Initializer

# init(display:including:)

Creates a filter that captures only specific windows from a display.

Mac Catalyst 18.2+macOS 12.3+

``` source
init(
    display: SCDisplay,
    including includedWindows: [SCWindow]
)
```

## Parameters 

`display`  

A display to capture.

`includedWindows`  

An array of windows to include in the output.

## See Also

### Creating a filter

init(desktopIndependentWindow: SCWindow)

Creates a filter that captures only the specified window.

init(display: SCDisplay, excludingWindows: [SCWindow])

Creates a filter that captures the contents of a display, excluding the specified windows.

init(display: SCDisplay, including: [SCRunningApplication], exceptingWindows: [SCWindow])

Creates a filter that captures a display, including only windows of the specified apps.

init(display: SCDisplay, excludingApplications: [SCRunningApplication], exceptingWindows: [SCWindow])

Creates a filter that captures a display, excluding windows of the specified apps.

