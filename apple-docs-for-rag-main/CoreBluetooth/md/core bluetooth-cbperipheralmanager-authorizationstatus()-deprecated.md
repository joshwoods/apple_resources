

- Core Bluetooth
- CBPeripheralManager
-  authorizationStatus() Deprecated

Type Method

# authorizationStatus()

Returns the app’s authorization status for sharing data while in the background.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
class func authorizationStatus() -> CBPeripheralManagerAuthorizationStatus
```

Deprecated

Use CBManagerAuthorization instead

## Return Value

A value that indicates whether the app has authorization to share data using Bluetooth services while in the background. For a list of possible values, see CBPeripheralManagerAuthorizationStatus.

## Discussion

The system manages the authorization status of a given app, and considers several factors. The user must explicitly authorize apps to share data using Bluetooth services while in the background state. The system automatically displays a request for user authorization when your app first attempts to use Bluetooth services to share data.

Calling this method doesn’t prompt the user for access. Instead, you use this method to detect restricted access and hide any affected UI features from the user.

## See Also

### Monitoring the State of a Peripheral Manager

enum CBPeripheralManagerAuthorizationStatus

Values representing the current authorization state of the peripheral manager.

Deprecated

enum CBPeripheralManagerState

Values that represent the current state of the peripheral manager.

Deprecated

