

- XCUIAutomation
- XCUIScreenshotProviding
-  screenshot() 

Instance Method

# screenshot()

Takes a screenshot of a screen or UI element’s current visual state.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func screenshot() -> XCUIScreenshot
```

**Required**

## Discussion

The output of this method is equivalent to capturing a screenshot manually on a device. For example, if you take a screenshot of a window on macOS that is covered by another window, the covering window is visible in the screenshot.

