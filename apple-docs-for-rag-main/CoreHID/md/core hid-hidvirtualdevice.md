

- Core HID
-  HIDVirtualDevice 

Class

# HIDVirtualDevice

A virtual service to emulate a HID device connected to the system.

macOS 15.0+

``` source
actor HIDVirtualDevice
```

## Mentioned in 

Creating virtual devices

## Overview

A HID device is a computer peripheral intended to provide direction to the system from human input. The specification is a broad, industry-wide standard maintained by the USB Implementers Forum.

A `HIDVirtualDevice` is an object that emulates a HID device connected to the system, without the need for a physical device. Such a tool can be used by an app to emulate a keyboard and dispatch HID reports to the system using dispatchInputReport(data:timestamp:) that signify key strokes, and could be received by a HIDDeviceClientlistening for such activity in other apps. The virtual device can also receive requests from the system using its HIDVirtualDeviceDelegate.

## Topics

### Create a HID virtual device

init?(properties: HIDVirtualDevice.Properties)

Creates a virtual HID device.

let deviceReference: HIDDeviceClient.DeviceReference

The reference to the virtual HID device.

func activate(delegate: any HIDVirtualDeviceDelegate)

Activate a newly created virtual device to begin receiving notifications and enable functionality.

### Dispatch input reports

func dispatchInputReport(data: Data, timestamp: SuspendingClock.Instant) async throws

Dispatch an input report to the system.

### Structures

struct Properties

The properties for a virtual HID device.

### Instance Properties

var unownedExecutor: UnownedSerialExecutor

Retrieve the executor for this actor as an optimized, unowned reference.

### Default Implementations

Actor Implementations

CustomStringConvertible Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Actor
- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Simulation

Creating virtual devices

Use and interact with a virtual human interface device for testing and development.

protocol HIDVirtualDeviceDelegate

The delegate to receive notifications for a virtual HID device.

struct Properties

The properties for a virtual HID device.

