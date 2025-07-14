

- WatchKit
-  WKInterfaceDevice 

Class

# WKInterfaceDevice

An object that provides information about the user’s Apple Watch.

watchOS 2.0+

``` source
class WKInterfaceDevice
```

## Overview

You can use the information from WKInterfaceDevice to make decisions about the content you display in your app. You can also use this object to play haptic feedback when your app is active.

Do not subclass or create instances of this class yourself. Always call the current() class method to get the shared device object.

## Topics

### Accessing the Shared Device Object

class func current() -> WKInterfaceDevice

Returns the shared device object.

### Reading the Screen Information

var screenBounds: CGRect

The bounding rectangle of the screen.

var screenScale: CGFloat

The number of pixels per point for the current screen.

### Reading the Device Settings

var name: String

The name of the device.

var model: String

The model information for the device.

var localizedModel: String

The localized version of the model information.

var wristLocation: WKInterfaceDeviceWristLocation

The wrist on which the user wears the Apple Watch.

enum WKInterfaceDeviceWristLocation

Constants indicating the wrist on which the user wears the Apple Watch.

var crownOrientation: WKInterfaceDeviceCrownOrientation

The side on which the crown is positioned.

enum WKInterfaceDeviceCrownOrientation

Constants indicating the crown orientation from the user’s perspective.

var preferredContentSizeCategory: String

The preferred font-sizing option.

### Reading System Information

var systemName: String

The name of the operating system.

var systemVersion: String

The version of the operating system.

### Accessing the Layout Direction

var layoutDirection: WKInterfaceLayoutDirection

The layout direction of the user interface.

class func interfaceLayoutDirection(for: WKInterfaceSemanticContentAttribute) -> WKInterfaceLayoutDirection

Returns the user interface direction for the given semantic content attribute.

enum WKInterfaceSemanticContentAttribute

A semantic description of the view’s contents, used to determine whether the view should be flipped when switching between left-to-right and right-to-left layouts.

enum WKInterfaceLayoutDirection

Specifies the directional flow of the user interface.

### Reading Information About the Battery

var isBatteryMonitoringEnabled: Bool

A Boolean value that determines whether the app can monitor the device’s battery.

var batteryLevel: Float

The battery’s current percent charge.

var batteryState: WKInterfaceDeviceBatteryState

The device’s battery state.

enum WKInterfaceDeviceBatteryState

The battery’s charging state.

### Accessing Water Resistance and Lock

var waterResistanceRating: WKWaterResistanceRating

The Apple Watch water-resistance rating.

enum WKWaterResistanceRating

Values indicating the water-resistance rating.

var isWaterLockEnabled: Bool

A Boolean value that indicates whether the water lock is enabled.

func enableWaterLock()

Disables the Apple Watch touch screen to prevent accidental taps while submerged.

### Playing Haptic Feedback

func play(WKHapticType)

Gives haptic feedback to the user.

enum WKHapticType

Constant indicating the style of feedback to deliver using haptics.

### Streaming Audio

var supportsAudioStreaming: Bool

A Boolean value that indicates whether the device supports audio streaming.

### Validating In-App Purchases

var identifierForVendor: UUID?

An alphanumeric string that uniquely identifies a device to the app’s vendor.

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

## See Also

### App structure

Setting up a watchOS project

Create a new watchOS project or add a watch target to an existing iOS project.

class WKApplication

The centralized point of control and coordination for apps with a single watchOS app target.

protocol WKApplicationDelegate

A collection of methods that manages the app-level behavior for a single-target watchOS app.

class WKExtension

The centralized point of control and coordination for extension-based apps running in watchOS.

protocol WKExtensionDelegate

A collection of methods that manages the app-level behavior of a WatchKit extension.

func WKApplicationMain(Int32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>, String?) -> Int32

Creates the application object and the application delegate, and sets up the app’s event cycle.

WKPrefersNetworkUponForeground

A Boolean value that indicates whether an app requires network access on launch.

