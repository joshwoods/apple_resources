

- Playground Bluetooth
-  PlaygroundBluetoothConnectionViewDataSource 

Protocol

# PlaygroundBluetoothConnectionViewDataSource

The protocol you adopt to display an available peripheral in a playground page’s connection view.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
protocol PlaygroundBluetoothConnectionViewDataSource : AnyObject
```

## Overview

The example below shows a conformance to this protocol that uses images from a playground book’s Public and Private Resources Folders.

extension PageViewDelegate: PlaygroundBluetoothConnectionViewDataSource {
    func connectionView(_ connectionView: PlaygroundBluetoothConnectionView, itemForPeripheral peripheral: CBPeripheral, withAdvertisementData advertisementData: [String: Any]?) -> PlaygroundBluetoothConnectionView.Item {
        let icon = UIImage(named: &quot;Peripheral_Icon_Normal&quot;)!
        let issueIcon = UIImage(named: &quot;Peripheral_Icon_Issue&quot;)!
        let name = peripheral.name ?? peripheral.identifier.uuidString

        return .init(name: name, icon: icon, issueIcon: issueIcon)
    }
}

Some peripherals have Bluetooth characteristics that provide information about the peripheral’s battery charge level or firmware status. Include this information in the PlaygroundBluetoothConnectionView.Item you create when it will help people pick a peripheral.

## Topics

### Displaying Connection View Items

func connectionView(PlaygroundBluetoothConnectionView, itemForPeripheral: CBPeripheral, withAdvertisementData: [String : Any]?) -> PlaygroundBluetoothConnectionView.Item

Tells the delegate that a new peripheral was discovered and can be displayed in the connection view.

**Required**

## See Also

### Peripheral Display

class PlaygroundBluetoothConnectionView

A view that displays the connection status of a peripheral to the central manager for the current page and manages connections to other peripherals.

protocol PlaygroundBluetoothConnectionViewDelegate

A delegate you use to respond to user- and system-initiated interactions with the central manager’s connection view.

