

- Network Extension
-  NEProviderStopReason 

Enumeration

# NEProviderStopReason

Reasons why the provider extension was stopped.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
enum NEProviderStopReason
```

## Overview

`NEProviderStopReasonUserLogout` and `NEProviderStopReasonUserSwitch` are available only in macOS.

## Topics

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

case connectionFailed

The connection failed.

case sleep

A stop reason indicating the configuration enabled disconnect on sleep and the device went to sleep.

### Enumeration Cases

case internalError

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

