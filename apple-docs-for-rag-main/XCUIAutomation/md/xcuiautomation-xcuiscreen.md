

- XCUIAutomation
-  XCUIScreen 

Class

# XCUIScreen

A physical screen attached to a device.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
class XCUIScreen
```

## Overview

Call the screenshot() method on an XCUIScreen instance to capture a screenshot of its current UI state. The XCUIScreenshotProviding protocol adds this method to XCUIScreen.

You can take a screenshot of the current device’s main screen using the following code:

```
let screenshot = XCUIScreen.main.screenshot()
```

You can take a screenshot of every screen on the current device using the following code:

```
let allScreenshots = XCUIScreen.screens.map { screen in
    return screen.screenshot()
}
```

## Topics

### Device screens

class var main: XCUIScreen

The current device’s main screen.

class var screens: [XCUIScreen]

The current device’s active screens.

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
- XCUIScreenshotProviding

## See Also

### Screenshots

class XCUIScreenshot

A captured image of a screen, app, or UI element state.

protocol XCUIScreenshotProviding

A type that can provide a screenshot of its current UI state.

