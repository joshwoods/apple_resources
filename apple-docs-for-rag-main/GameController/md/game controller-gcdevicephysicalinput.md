

- Game Controller
-  GCDevicePhysicalInput 

Protocol

# GCDevicePhysicalInput

The common properties and methods for objects that represent the input profile of a device.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol GCDevicePhysicalInput : GCDevicePhysicalInputState
```

## Mentioned in 

Handling input events

## Overview

You can safely call this protocol’s methods and access its properties from any thread, but not from multiple, concurrent threads.

## Topics

### Getting the device

var device: (any GCDevice)?

The device that the physical input represents.

**Required**

### Handling device input

func nextInputState() -> (any GCDevicePhysicalInputState &amp; GCDevicePhysicalInputStateDiff)?

Returns the next input state from the queue.

**Required**

var inputStateAvailableHandler: ((any GCDevicePhysicalInput) -> Void)?

The block that the profile calls when Game Controller adds an input state to the queue.

**Required**

var inputStateQueueDepth: Int

The maximum number of input values that the queue stores.

**Required**

func capture() -> any GCDevicePhysicalInputState

Returns a snapshot of the physical device inputs.

**Required**

var elementValueDidChangeHandler: ((any GCDevicePhysicalInput, any GCPhysicalInputElement) -> Void)?

A block that the profile calls when an element’s value changes.

**Required**

### Changing the callback dispatch queue

var queue: dispatch_queue_t?

The dispatch queue that the system uses for callbacks.

**Required**

## Relationships

### Inherits From

- GCDevicePhysicalInputState
- NSObjectProtocol

### Conforming Types

- GCControllerLiveInput
- GCRacingWheelInput

## See Also

### Essentials

Handling input events

Receive controller input using either polling or callbacks.

protocol GCDevicePhysicalInputState

The common properties for physical devices with elements.

protocol GCDevicePhysicalInputStateDiff

The common functions for objects that contain the differences between a current and previous input state object.

