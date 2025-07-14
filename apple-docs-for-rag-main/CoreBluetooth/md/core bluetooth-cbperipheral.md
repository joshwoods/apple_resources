

- Core Bluetooth
-  CBPeripheral 

Class

# CBPeripheral

A remote peripheral device.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CBPeripheral
```

## Overview

The CBPeripheral class represents remote peripheral devices that your app discovers with a central manager (an instance of CBCentralManager). Peripherals use universally unique identifiers (UUIDs), represented by NSUUID objects, to identify themselves. Peripherals may contain one or more services or provide useful information about their connected signal strength.

You use this class to discover, explore, and interact with the services available on a remote peripheral that supports Bluetooth low energy. A service encapsulates the way part of the device behaves. For example, one service of a heart rate monitor may be to expose heart rate data from a sensor. Services themselves contain of characteristics or included services (references to other services). Characteristics provide further details about a peripheral’s service. For example, the heart rate service may contain multiple characteristics. One characteristic could describe the intended body location of the device’s heart rate sensor, and another characteristic could transmit the heart rate measurement data. Finally, characteristics contain any number of descriptors that provide more information about the characteristic’s value, such as a human-readable description and a way to format the value.

## Topics

### Identifying a Peripheral

var name: String?

The name of the peripheral.

var delegate: (any CBPeripheralDelegate)?

The delegate object specified to receive peripheral events.

### Discovering Services

func discoverServices([CBUUID]?)

Discovers the specified services of the peripheral.

func discoverIncludedServices([CBUUID]?, for: CBService)

Discovers the specified included services of a previously-discovered service.

var services: [CBService]?

A list of a peripheral’s discovered services.

### Discovering Characteristics and Descriptors

func discoverCharacteristics([CBUUID]?, for: CBService)

Discovers the specified characteristics of a service.

func discoverDescriptors(for: CBCharacteristic)

Discovers the descriptors of a characteristic.

### Reading Characteristic and Descriptor Values

func readValue(for: CBCharacteristic)

Retrieves the value of a specified characteristic.

func readValue(for: CBDescriptor)

Retrieves the value of a specified characteristic descriptor.

### Writing Characteristic and Descriptor Values

func writeValue(Data, for: CBCharacteristic, type: CBCharacteristicWriteType)

Writes the value of a characteristic.

func writeValue(Data, for: CBDescriptor)

Writes the value of a characteristic descriptor.

func maximumWriteValueLength(for: CBCharacteristicWriteType) -> Int

The maximum amount of data, in bytes, you can send to a characteristic in a single write type.

enum CBCharacteristicWriteType

Values representing the possible write types to a characteristic’s value.

### Setting Notifications for a Characteristic’s Value

func setNotifyValue(Bool, for: CBCharacteristic)

Sets notifications or indications for the value of a specified characteristic.

### Monitoring a Peripheral’s Connection State

var state: CBPeripheralState

The connection state of the peripheral.

enum CBPeripheralState

Values representing the connection state of a peripheral.

var canSendWriteWithoutResponse: Bool

A Boolean value that indicates whether the remote device can send a write without a response.

### Accessing a Peripheral’s Signal Strength

func readRSSI()

Retrieves the current RSSI value for the peripheral while connected to the central manager.

var rssi: NSNumber?

The Received Signal Strength Indicator (RSSI), in decibels, of the peripheral.

Deprecated

### Working with L2CAP Channels

func openL2CAPChannel(CBL2CAPPSM)

Attempts to open an L2CAP channel to the peripheral using the supplied Protocol/Service Multiplexer (PSM).

class CBL2CAPChannel

A live L2CAP connection to a remote device.

typealias CBL2CAPPSM

The type of PSM identifiers.

### Working with Apple Notification Center Service (ANCS)

var ancsAuthorized: Bool

A Boolean value that indicates if the remote device has authorization to receive data over ANCS protocol.

## Relationships

### Inherits From

- CBPeer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Peripherals

protocol CBPeripheralDelegate

A protocol that provides updates on the use of a peripheral’s services.

class CBPeripheralManager

An object that manages and advertises peripheral services exposed by this app.

protocol CBPeripheralManagerDelegate

A protocol that provides updates for local peripheral state and interactions with remote central devices.

class CBAttribute

A representation of common aspects of services offered by a peripheral.

struct CBAttributePermissions

Values that represent the read, write, and encryption permissions for a characteristic’s value.

