

- External Accessory
-  EAWiFiUnconfiguredAccessoryProperties 

Structure

# EAWiFiUnconfiguredAccessoryProperties

Options that can be combined using the C bitwise `OR` operator to represent the properties of an unconfigured accessory.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
struct EAWiFiUnconfiguredAccessoryProperties
```

## Topics

### Getting the Accessory Properties

static var propertySupportsAirPlay: EAWiFiUnconfiguredAccessoryProperties

The accessory indicates that it supports AirPlay.

static var propertySupportsAirPrint: EAWiFiUnconfiguredAccessoryProperties

The accessory indicates that it supports AirPrint.

static var propertySupportsHomeKit: EAWiFiUnconfiguredAccessoryProperties

The accessory indicates that it supports HomeKit.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Getting Information About the Accessory

var name: String

The name of the accessory.

var manufacturer: String

The name of the accessory’s manufacturer.

var model: String

The model name of accessory.

var ssid: String

The Wi-Fi SSID of the accessory.

var macAddress: String

The primary MAC address of the accessory.

var properties: EAWiFiUnconfiguredAccessoryProperties

The properties the accessory supports.

