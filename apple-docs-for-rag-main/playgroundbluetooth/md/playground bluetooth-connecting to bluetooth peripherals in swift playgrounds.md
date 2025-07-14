

- Playground Bluetooth
-  Connecting to Bluetooth Peripherals in Swift Playgrounds 

Article

# Connecting to Bluetooth Peripherals in Swift Playgrounds

Scan for peripherals and display them in your playground's live view.

## Overview

Playgrounds use Bluetooth to connect to nearby peripherals to send and receive commands or data. You can incorporate periperals into your playground to have your users learn programming concepts by interacting with real-world objects.

### Scan for Peripherals

You use a PlaygroundBluetoothCentralManager to scan for and connect to nearby Bluetooth peripherals. It automatically stores the ID of the most recently connected peripheral. The example below scans for all kinds of peripherals by passing `nil` to the initializer for the PlaygroundBluetoothCentralManagerDelegate.

Once you determine which Bluetooth services your playground page requires, instead of passing `nil` for those services, pass an array of CBUUID instances.

### Display Peripherals in a Live View

You use a PlaygroundBluetoothConnectionView to display status information about nearby peripherals. The example belows shows how to configure and place a connection view on a playground page.

Important

Always use the system-provided `PlaygroundBluetoothConnectionView` to display connection information for peripherals. Doing so helps provide a consistent experience for people who also use playground books created by others.

## See Also

### Peripheral Connection

class PlaygroundBluetoothCentralManager

A streamlined interface for connecting the central manager for the current playground page to nearby Bluetooth peripherals.

protocol PlaygroundBluetoothCentralManagerDelegate

A delegate you use to respond to peripheral discovery and manage the lifecycle of connections.

