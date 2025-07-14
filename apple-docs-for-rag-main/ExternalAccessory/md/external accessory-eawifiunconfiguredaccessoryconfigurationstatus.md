

- External Accessory
-  EAWiFiUnconfiguredAccessoryConfigurationStatus 

Enumeration

# EAWiFiUnconfiguredAccessoryConfigurationStatus

Values that represent the state of the configuration process for an EAWiFiUnconfiguredAccessory object.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
enum EAWiFiUnconfiguredAccessoryConfigurationStatus
```

## Topics

### Status Values

case success

The configuration of the accessory succeeded.

case userCancelledConfiguration

The user cancelled the configuration process.

case failed

The configuration failed.

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

### Getting Updates About the Configuration Process

func accessoryBrowser(EAWiFiUnconfiguredAccessoryBrowser, didFinishConfiguringAccessory: EAWiFiUnconfiguredAccessory, with: EAWiFiUnconfiguredAccessoryConfigurationStatus)

Indicates that the browser has completed configuring the specified accessory.

**Required**

