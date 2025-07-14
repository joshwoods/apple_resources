

- Core Bluetooth
- CBPeripheralManagerAuthorizationStatus
-  CBPeripheralManagerAuthorizationStatus.restricted Deprecated

Case

# CBPeripheralManagerAuthorizationStatus.restricted

An authorization status that indicates this app isn’t authorized to share data using Bluetooth while in the background.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
case restricted
```

Deprecated

Use CBManagerAuthorization instead

## Discussion

The user can’t change this app’s status, possibly due to active restrictions such as parental controls being in place.

## See Also

### Constants

case notDetermined

An authorization status that indicates the user hasn’t indicated whether this app can share data using Bluetooth while in the background.

Deprecated

case denied

An authorization status that indicates the user explicitly denied this app from sharing data using Bluetooth while in the background.

Deprecated

case authorized

An authorization status that indicates the user authorized this app to share data using Bluetooth while in the background.

Deprecated

