

- Playground Bluetooth
-  PlaygroundBluetoothConnectionView 

Class

# PlaygroundBluetoothConnectionView

A view that displays the connection status of a peripheral to the central manager for the current page and manages connections to other peripherals.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
class PlaygroundBluetoothConnectionView : UIView
```

## Overview

The view can display peripheral names, icons, connection statuses, and battery levels.

Figure 1 A PlaygroundBluetoothConnectionView instance in the peripheral selection state.

## Topics

### Creating Connection Views

init(centralManager: PlaygroundBluetoothCentralManager, delegate: PlaygroundBluetoothConnectionViewDelegate?, dataSource: PlaygroundBluetoothConnectionViewDataSource?)

Creates a new, empty view that can be populated with items when peripherals are connected to the central manager.

init?(coder: NSCoder)

Creates a connection view initialized from data you supply.

var dataSource: PlaygroundBluetoothConnectionViewDataSource?

A data source that provides subviews for available peripherals.

### Displaying Peripherals

func setItem(PlaygroundBluetoothConnectionView.Item, forPeripheral: CBPeripheral)

Sets all of the information about the specified peripheral at once.

struct PlaygroundBluetoothConnectionView.Item

A value that holds information about a peripheral displayed in a connection view.

### Handling State Changes

var delegate: PlaygroundBluetoothConnectionViewDelegate?

A delegate you supply to make decisions about which peripherals are displayed in the view.

enum PlaygroundBluetoothConnectionView.State

The states that tell users how to proceed when connecting to and switching between peripherals in a playground page.

### Displaying Individual Details

func setBatteryLevel(Double?, forPeripheral: CBPeripheral)

Displays the battery level for the specified peripheral.

func setFirmwareStatus(PlaygroundBluetoothConnectionView.Item.FirmwareStatus?, forPeripheral: CBPeripheral)

Displays whether or not the specified peripheral’s firmware is up-to-date.

func setIcon(UIImage, forPeripheral: CBPeripheral)

Displays an icon representing the specified peripheral.

func setIssueIcon(UIImage, forPeripheral: CBPeripheral)

Displays an icon indicating that the specified peripheral is available but may not be usable.

func setName(String, forPeripheral: CBPeripheral)

Displays the name of the specified peripheral.

## Relationships

### Inherits From

- UIView

## See Also

### Peripheral Display

protocol PlaygroundBluetoothConnectionViewDelegate

A delegate you use to respond to user- and system-initiated interactions with the central manager’s connection view.

protocol PlaygroundBluetoothConnectionViewDataSource

The protocol you adopt to display an available peripheral in a playground page’s connection view.

