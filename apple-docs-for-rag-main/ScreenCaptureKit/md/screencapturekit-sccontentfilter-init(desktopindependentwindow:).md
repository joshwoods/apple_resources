

- ScreenCaptureKit
- SCContentFilter
-  init(desktopIndependentWindow:) 

Initializer

# init(desktopIndependentWindow:)

Creates a filter that captures only the specified window.

Mac Catalyst 18.2+macOS 12.3+

``` source
init(desktopIndependentWindow window: SCWindow)
```

## Parameters 

`window`  

A window to capture.

## See Also

### Creating a filter

init(display: SCDisplay, including: [SCWindow])

Creates a filter that captures only specific windows from a display.

init(display: SCDisplay, excludingWindows: [SCWindow])

Creates a filter that captures the contents of a display, excluding the specified windows.

init(display: SCDisplay, including: [SCRunningApplication], exceptingWindows: [SCWindow])

Creates a filter that captures a display, including only windows of the specified apps.

init(display: SCDisplay, excludingApplications: [SCRunningApplication], exceptingWindows: [SCWindow])

Creates a filter that captures a display, excluding windows of the specified apps.

