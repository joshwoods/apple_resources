

- XCUIAutomation
- XCUIScreen
-  main 

Type Property

# main

The current device’s main screen.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
class var main: XCUIScreen { get }
```

## Discussion

On macOS, main represents the screen that owns the menu bar. On iOS and tvOS, main represents the primary screen of the device.

## See Also

### Device screens

class var screens: [XCUIScreen]

The current device’s active screens.

