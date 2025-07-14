

- ScreenCaptureKit
- SCContentFilter
-  init(display:excludingWindows:) 

Initializer

# init(display:excludingWindows:)

Creates a filter that captures the contents of a display, excluding the specified windows.

Mac Catalyst 18.2+macOS 12.3+

``` source
init(
    display: SCDisplay,
    excludingWindows excluded: [SCWindow]
)
```

## Parameters 

`display`  

A display to capture.

`excluded`  

An array of windows to exclude from the output.

## See Also

### Creating a filter

init(desktopIndependentWindow: SCWindow)

Creates a filter that captures only the specified window.

init(display: SCDisplay, including: [SCWindow])

Creates a filter that captures only specific windows from a display.

init(display: SCDisplay, including: [SCRunningApplication], exceptingWindows: [SCWindow])

Creates a filter that captures a display, including only windows of the specified apps.

init(display: SCDisplay, excludingApplications: [SCRunningApplication], exceptingWindows: [SCWindow])

Creates a filter that captures a display, excluding windows of the specified apps.

