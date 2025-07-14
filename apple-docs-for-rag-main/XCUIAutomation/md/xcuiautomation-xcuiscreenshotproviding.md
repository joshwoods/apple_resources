

- XCUIAutomation
-  XCUIScreenshotProviding 

Protocol

# XCUIScreenshotProviding

A type that can provide a screenshot of its current UI state.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
protocol XCUIScreenshotProviding : NSObjectProtocol
```

## Overview

Call this protocol’s screenshot() method on an XCUIScreen or XCUIElement to capture a screenshot of its current UI state.

## Topics

### Taking a Screenshot

func screenshot() -> XCUIScreenshot

Takes a screenshot of a screen or UI element’s current visual state.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- XCUIApplication
- XCUIElement
- XCUIScreen

## See Also

### Screenshots

class XCUIScreen

A physical screen attached to a device.

class XCUIScreenshot

A captured image of a screen, app, or UI element state.

