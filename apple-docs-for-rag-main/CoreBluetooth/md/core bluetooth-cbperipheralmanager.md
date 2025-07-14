

- Core Bluetooth
-  CBPeripheralManager 

Class

# CBPeripheralManager

An object that manages and advertises peripheral services exposed by this app.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CBPeripheralManager
```

## Overview

Core Bluetooth uses CBPeripheralManager objects to manage published services within the local peripheral’s Generic Attribute Profile (GATT) database and to advertise these services to central devices (represented by CBCentral objects). While a service is in the database, any connected central can see and connect to it. That said, if your app hasn’t specified the `bluetooth-peripheral` background mode, the contents of its services become disabled when it’s in the background or in a suspended state. In this scenario, any remote central trying to access the service’s characteristic value or characteristic descriptors receives an error.

Before you call CBPeripheralManager methods, the peripheral manager object must be in the powered-on state, as indicated by the CBPeripheralManagerState.poweredOn. This state indicates that the device (your iPhone or iPad, for instance) supports Bluetooth low energy and that its Bluetooth is on and available for use.

In watchOS, tvOS, and visionOS, you can’t advertise services using a CBPeripheralManager object because support for doing so is unavailable.

## Topics

### Initializing a Peripheral Manager

convenience init()

Initializes the peripheral manager without a delegate.

convenience init(delegate: (any CBPeripheralManagerDelegate)?, queue: dispatch_queue_t?)

Initializes the peripheral manager with a specified delegate and dispatch queue.

init(delegate: (any CBPeripheralManagerDelegate)?, queue: dispatch_queue_t?, options: [String : Any]?)

Initializes the peripheral manager with a specified delegate, dispatch queue, and initialization options.

var delegate: (any CBPeripheralManagerDelegate)?

The delegate object specified to receive peripheral events.

Peripheral Manager Initialization Options

Keys used to specify options when creating a peripheral manager.

### Monitoring the State of a Peripheral Manager

class func authorizationStatus() -> CBPeripheralManagerAuthorizationStatus

Returns the app’s authorization status for sharing data while in the background.

Deprecated

enum CBPeripheralManagerAuthorizationStatus

Values representing the current authorization state of the peripheral manager.

Deprecated

enum CBPeripheralManagerState

Values that represent the current state of the peripheral manager.

Deprecated

### Adding and Removing Services

func add(CBMutableService)

Publishes a service and any of its associated characteristics and characteristic descriptors to the local GATT database.

func remove(CBMutableService)

Removes a specified published service from the local GATT database.

func removeAllServices()

Removes all published services from the local GATT database.

### Managing Advertising

func startAdvertising([String : Any]?)

Advertises peripheral manager data.

Advertising Data

func stopAdvertising()

Stops advertising peripheral manager data.

var isAdvertising: Bool

A Boolean value that indicates whether the peripheral is advertising data.

### Sending Updates of a Characteristic’s Value

func updateValue(Data, for: CBMutableCharacteristic, onSubscribedCentrals: [CBCentral]?) -> Bool

Send an updated characteristic value to one or more subscribed centrals, using a notification or indication.

### Responding to Read and Write Requests

func respond(to: CBATTRequest, withResult: CBATTError.Code)

Responds to a read or write request from a connected central.

### Setting Connection Latency

func setDesiredConnectionLatency(CBPeripheralManagerConnectionLatency, for: CBCentral)

Sets the desired connection latency for an existing connection to a central device.

enum CBPeripheralManagerConnectionLatency

Values representing the connection latency of the peripheral manager.

### Using L2CAP Channels

func publishL2CAPChannel(withEncryption: Bool)

Creates a listener for incoming L2CAP channel connections.

func unpublishL2CAPChannel(CBL2CAPPSM)

Removes a published service from the local system.

## Relationships

### Inherits From

- CBManager

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Peripherals

class CBPeripheral

A remote peripheral device.

protocol CBPeripheralDelegate

A protocol that provides updates on the use of a peripheral’s services.

protocol CBPeripheralManagerDelegate

A protocol that provides updates for local peripheral state and interactions with remote central devices.

class CBAttribute

A representation of common aspects of services offered by a peripheral.

struct CBAttributePermissions

Values that represent the read, write, and encryption permissions for a characteristic’s value.

