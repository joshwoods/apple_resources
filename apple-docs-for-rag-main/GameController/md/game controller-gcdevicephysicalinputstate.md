

- Game Controller
-  GCDevicePhysicalInputState 

Protocol

# GCDevicePhysicalInputState

The common properties for physical devices with elements.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol GCDevicePhysicalInputState : NSObjectProtocol
```

## Mentioned in 

Handling input events

## Overview

It’s safe to call any property and method implementation of this protocol from any thread, as long as you don’t do so from multiple threads concurrently.

## Topics

### Getting the device

var device: (any GCDevice)?

The physical device that this profile represents.

**Required**

### Getting change information

var lastEventTimestamp: TimeInterval

The time of the most recent event.

**Required**

var lastEventLatency: TimeInterval

The time in seconds between the last event and the current time.

**Required**

### Accessing elements

var elements: GCPhysicalInputElementCollection&lt;any GCPhysicalInputElement>

The device’s elements as key-value pairs for lookup by name.

var axes: GCPhysicalInputElementCollection&lt;any GCAxisElement>

The device’s axes as key-value pairs for lookup by name.

var buttons: GCPhysicalInputElementCollection&lt;any GCButtonElement>

The device’s buttons as key-value pairs for lookup by name.

var dpads: GCPhysicalInputElementCollection&lt;any GCDirectionPadElement>

The device’s directional pads as key-value pairs for lookup by name.

var switches: GCPhysicalInputElementCollection&lt;any GCSwitchElement>

The device’s switches as key-value pairs for lookup by name.

subscript(String) -> (any GCPhysicalInputElement)?

Returns the element that the key specifies.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- GCDevicePhysicalInput

### Conforming Types

- GCControllerInputState
- GCControllerLiveInput
- GCRacingWheelInput
- GCRacingWheelInputState

## See Also

### Essentials

Handling input events

Receive controller input using either polling or callbacks.

protocol GCDevicePhysicalInput

The common properties and methods for objects that represent the input profile of a device.

protocol GCDevicePhysicalInputStateDiff

The common functions for objects that contain the differences between a current and previous input state object.

