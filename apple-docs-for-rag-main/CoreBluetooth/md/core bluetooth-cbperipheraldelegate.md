

- Core Bluetooth
-  CBPeripheralDelegate 

Protocol

# CBPeripheralDelegate

A protocol that provides updates on the use of a peripheral’s services.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
protocol CBPeripheralDelegate : NSObjectProtocol
```

## Overview

The delegate of a CBPeripheral object must adopt the CBPeripheralDelegate protocol. The delegate uses this protocol’s methods to monitor the discovery, exploration, and interaction of a remote peripheral’s services and properties. This protocol doesn’t have any required methods.

## Topics

### Discovering Services

func peripheral(CBPeripheral, didDiscoverServices: (any Error)?)

Tells the delegate that peripheral service discovery succeeded.

func peripheral(CBPeripheral, didDiscoverIncludedServicesFor: CBService, error: (any Error)?)

Tells the delegate that discovering included services within the indicated service completed.

### Discovering Characteristics and their Descriptors

func peripheral(CBPeripheral, didDiscoverCharacteristicsFor: CBService, error: (any Error)?)

Tells the delegate that the peripheral found characteristics for a service.

func peripheral(CBPeripheral, didDiscoverDescriptorsFor: CBCharacteristic, error: (any Error)?)

Tells the delegate that the peripheral found descriptors for a characteristic.

### Retrieving Characteristic and Descriptor Values

func peripheral(CBPeripheral, didUpdateValueFor: CBCharacteristic, error: (any Error)?)

Tells the delegate that retrieving the specified characteristic’s value succeeded, or that the characteristic’s value changed.

func peripheral(CBPeripheral, didUpdateValueFor: CBDescriptor, error: (any Error)?)

Tells the delegate that retrieving a specified characteristic descriptor’s value succeeded.

### Writing Characteristic and Descriptor Values

func peripheral(CBPeripheral, didWriteValueFor: CBCharacteristic, error: (any Error)?)

Tells the delegate that the peripheral successfully set a value for the characteristic.

func peripheral(CBPeripheral, didWriteValueFor: CBDescriptor, error: (any Error)?)

Tells the delegate that the peripheral successfully set a value for the descriptor.

func peripheralIsReady(toSendWriteWithoutResponse: CBPeripheral)

Tells the delegate that a peripheral is again ready to send characteristic updates.

### Managing Notifications for a Characteristic’s Value

func peripheral(CBPeripheral, didUpdateNotificationStateFor: CBCharacteristic, error: (any Error)?)

Tells the delegate that the peripheral received a request to start or stop providing notifications for a specified characteristic’s value.

### Retrieving a Peripheral’s RSSI Data

func peripheral(CBPeripheral, didReadRSSI: NSNumber, error: (any Error)?)

Tells the delegate that retrieving the value of the peripheral’s current Received Signal Strength Indicator (RSSI) succeeded.

func peripheralDidUpdateRSSI(CBPeripheral, error: (any Error)?)

Tells the delegate that retrieving the value of the peripheral’s current Received Signal Strength Indicator (RSSI) succeeded.

Deprecated

### Monitoring Changes to a Peripheral’s Name or Services

func peripheralDidUpdateName(CBPeripheral)

Tells the delegate that a peripheral’s name changed.

func peripheral(CBPeripheral, didModifyServices: [CBService])

Tells the delegate that a peripheral’s services changed.

### Monitoring L2CAP Channels

func peripheral(CBPeripheral, didOpen: CBL2CAPChannel?, error: (any Error)?)

Delivers the result of an attempt to open an L2CAP channel.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Peripherals

class CBPeripheral

A remote peripheral device.

class CBPeripheralManager

An object that manages and advertises peripheral services exposed by this app.

protocol CBPeripheralManagerDelegate

A protocol that provides updates for local peripheral state and interactions with remote central devices.

class CBAttribute

A representation of common aspects of services offered by a peripheral.

struct CBAttributePermissions

Values that represent the read, write, and encryption permissions for a characteristic’s value.

