

- Core Bluetooth
-  CBCentralManagerDelegate 

Protocol

# CBCentralManagerDelegate

A protocol that provides updates for the discovery and management of peripheral devices.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
protocol CBCentralManagerDelegate : NSObjectProtocol
```

## Overview

The CBCentralManagerDelegate protocol defines the methods that a delegate of a CBCentralManager object must adopt. The optional methods of the protocol allow the delegate to monitor the discovery, connectivity, and retrieval of peripheral devices. The only required method is centralManagerDidUpdateState(_:); the central manager calls this when its state updates, thereby indicating the availability of the central manager.

## Topics

### Monitoring Connections with Peripherals

func centralManager(CBCentralManager, didConnect: CBPeripheral)

Tells the delegate that the central manager connected to a peripheral.

func centralManager(CBCentralManager, didDisconnectPeripheral: CBPeripheral, error: (any Error)?)

Tells the delegate that the central manager disconnected from a peripheral.

func centralManager(CBCentralManager, didFailToConnect: CBPeripheral, error: (any Error)?)

Tells the delegate the central manager failed to create a connection with a peripheral.

func centralManager(CBCentralManager, connectionEventDidOccur: CBConnectionEvent, for: CBPeripheral)

Tells the delegate that a connection event occurred which matches the registered options.

### Discovering and Retrieving Peripherals

func centralManager(CBCentralManager, didDiscover: CBPeripheral, advertisementData: [String : Any], rssi: NSNumber)

Tells the delegate the central manager discovered a peripheral while scanning for devices.

Advertisement Data Retrieval Keys

Keys used to specify items in a dictionary of peripheral advertisement data.

### Monitoring the Central Manager’s State

func centralManagerDidUpdateState(CBCentralManager)

Tells the delegate the central manager’s state updated.

**Required**

func centralManager(CBCentralManager, willRestoreState: [String : Any])

Tells the delegate the system is about to restore the central manager, as part of relaunching the app into the background.

### Monitoring the Central Manager’s Authorization

func centralManager(CBCentralManager, didUpdateANCSAuthorizationFor: CBPeripheral)

Tells the delegate the authorization status changed for a ANCS-requiring connected peripheral.

### Instance Methods

func centralManager(CBCentralManager, didDisconnectPeripheral: CBPeripheral, timestamp: CFAbsoluteTime, isReconnecting: Bool, error: (any Error)?)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Centrals

class CBCentral

A remote device connected to a local app, which is acting as a peripheral.

class CBCentralManager

An object that scans for, discovers, connects to, and manages peripherals.

