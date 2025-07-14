

- Network Extension
- NEProviderStopReason
-  NEProviderStopReason.sleep 

Case

# NEProviderStopReason.sleep

A stop reason indicating the configuration enabled disconnect on sleep and the device went to sleep.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 17.0+visionOS 1.0+

``` source
case sleep
```

## See Also

### Stop Reasons

case none

No specific reason.

case userInitiated

The user stopped the provider extension.

case providerFailed

The provider failed to function correctly.

case noNetworkAvailable

No network connectivity is currently available.

case unrecoverableNetworkChange

The device’s network connectivity changed.

case providerDisabled

The provider was disabled.

case authenticationCanceled

The authentication process was canceled.

case configurationFailed

The configuration is invalid.

case idleTimeout

The session timed out.

case configurationDisabled

The configuration was disabled.

case configurationRemoved

The configuration was removed.

case superceded

The configuration was superceded by a higher-priority configuration.

case userLogout

The user logged out.

case userSwitch

The current console user changed.

case appUpdate

