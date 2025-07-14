

- Core Bluetooth
- CBCentralManager
-  Peripheral Connection Options 

API Collection

# Peripheral Connection Options

Keys used to pass options when connecting to a peripheral.

## Topics

### Options

let CBConnectPeripheralOptionEnableAutoReconnect: String

A Boolean value that specifies whether the system automatically reconnects with a peripheral.

let CBConnectPeripheralOptionEnableTransportBridgingKey: String

An option to bridge classic Bluetooth technology profiles, if already connected over Bluetooth Low Energy.

let CBConnectPeripheralOptionNotifyOnConnectionKey: String

A Boolean value that specifies whether the system should display an alert when connecting a peripheral in the background.

let CBConnectPeripheralOptionNotifyOnDisconnectionKey: String

A Boolean value that specifies whether the system should display an alert when disconnecting a peripheral in the background.

let CBConnectPeripheralOptionNotifyOnNotificationKey: String

A Boolean value that specifies whether the system should display an alert for any notification sent by a peripheral.

let CBConnectPeripheralOptionRequiresANCS: String

An option to require Apple Notification Center Service (ANCS) when connecting a device.

let CBConnectPeripheralOptionStartDelayKey: String

An option that indicates a delay before the system makes a connection.

## See Also

### Establishing or Canceling Connections with Peripherals

func connect(CBPeripheral, options: [String : Any]?)

Establishes a local connection to a peripheral.

func cancelPeripheralConnection(CBPeripheral)

Cancels an active or pending local connection to a peripheral.

