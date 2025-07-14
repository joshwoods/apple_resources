

- External Accessory
-  EAWiFiUnconfiguredAccessoryBrowserState 

Enumeration

# EAWiFiUnconfiguredAccessoryBrowserState

The possible states of an accessory browser.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
enum EAWiFiUnconfiguredAccessoryBrowserState
```

## Topics

### States

case wiFiUnavailable

Wi-Fi is unavailable, typically because the user has placed the device in Airplane Mode or explicitly turned off Wi-Fi.

case stopped

The browser is not actively searching for unconfigured accessories.

case searching

The browser is actively searching for unconfigured accessory.

case configuring

The browser is actively configuring an accessory.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Updates About Browser State

func accessoryBrowser(EAWiFiUnconfiguredAccessoryBrowser, didUpdate: EAWiFiUnconfiguredAccessoryBrowserState)

Indicates that the browser’s state has changed.

**Required**

