

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
-  PlaygroundBluetoothConnectionView.State 

Enumeration

# PlaygroundBluetoothConnectionView.State

The states that tell users how to proceed when connecting to and switching between peripherals in a playground page.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
enum PlaygroundBluetoothConnectionView.State
```

## Overview

The example below shows how to use the different states as part of adopting the PlaygroundBluetoothConnectionViewDelegate protocol.

extension PageViewDelegate: PlaygroundBluetoothConnectionViewDelegate {
    func connectionView(_ connectionView: PlaygroundBluetoothConnectionView, titleFor state: PlaygroundBluetoothConnectionView.State) -> String {
        // Pick a name that matches the types of peripheral your playground
        // supports, such as &quot;Robot&quot;, &quot;Speaker&quot;, or &quot;Light&quot;.
        let name = &quot;Peripheral&quot;
        switch state {
        case .noConnection:
            return &quot;Connect \(name)&quot;
        case .connecting:
            return &quot;Connecting \(name)&quot;
        case .searchingForPeripherals:
            return &quot;Searching for \(name)s&quot;
        case .selectingPeripherals:
            return &quot;Select a \(name)&quot;
        case .connectedPeripheralFirmwareOutOfDate:
            return &quot;Connect to a Different \(name)&quot;
        }
    }
}

## Topics

### Waiting for Connections

case connecting

The peripheral is in the process of connecting to a connection view’s central manager.

case noConnection

The connection to a peripheral has been lost.

case searchingForPeripherals

A connection view’s central manager is scanning for nearby peripherals.

### Selecting Connections

case selectingPeripherals

One or more peripherals have been discovered and can be selected.

### Handling Old Firmware

case connectedPeripheralFirmwareOutOfDate

The currently connected peripheral has outdated firmware and can't be used.

### Comparing Connection States

static func != (PlaygroundBluetoothConnectionView.State, PlaygroundBluetoothConnectionView.State) -> Bool

Compares two connection states and returns `true` if they're different.

## See Also

### Handling State Changes

var delegate: PlaygroundBluetoothConnectionViewDelegate?

A delegate you supply to make decisions about which peripherals are displayed in the view.

