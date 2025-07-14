

- XCUIAutomation
-  XCUIScreenshot 

Class

# XCUIScreenshot

A captured image of a screen, app, or UI element state.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
class XCUIScreenshot
```

## Overview

Screenshots capture the current UI state of classes that conform to the XCUIScreenshotProviding protocol, such as XCUIScreen and XCUIElement. Each screenshot contains an image representation of the captured UI at the point the screenshot was taken.

The following code demonstrates taking screenshots of a screen and a UI element:

```
func testTakeScreenshots() {

    // Take a screenshot of the current device's main screen.
    let mainScreenScreenshot = XCUIScreen.main.screenshot()

    // Take a screenshot of an app's first window.
    let app = XCUIApplication()
    app.launch()
    let windowScreenshot = app.windows.firstMatch.screenshot()

}
```

If you use XCTest for your UI automation tests, you can attach a screenshot of your app’s UI to a test or activity to store it for later analysis. Create an attachment for a screenshot by calling the XCTAttachment initializer init(screenshot:) or init(screenshot:quality:). Add the attachment to a test or activity by calling the XCTActivity method add(_:). For more information, see Adding Attachments to Tests, Activities, and Issues.

## Topics

### Screenshot representations

var image: UIImage

A representation of the screenshot as a platform-native image object.

var pngRepresentation: Data

A representation of the screenshot as PNG image data.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Screenshots

class XCUIScreen

A physical screen attached to a device.

protocol XCUIScreenshotProviding

A type that can provide a screenshot of its current UI state.

