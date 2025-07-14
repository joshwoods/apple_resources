

- Game Controller
-  GCDevicePhysicalInputStateDiff 

Protocol

# GCDevicePhysicalInputStateDiff

The common functions for objects that contain the differences between a current and previous input state object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol GCDevicePhysicalInputStateDiff : NSObjectProtocol
```

## Overview

Use the `GCDevicePhysicalInput` nextInputState() method to get an input state object conforming to this protocol.

## Topics

### Getting changes

func change(for: any GCPhysicalInputElement) -> GCDevicePhysicalInputElementChange

Returns whether the input value of an element changes.

**Required**

enum GCDevicePhysicalInputElementChange

Possible values that describe whether the input value of an element changes.

func changedElements() -> NSEnumerator?

Returns the elements that changed since the previous input state.

func changedElements() -> (some Sequence&lt;any GCPhysicalInputElement>)? 

Returns the elements that changed since the previous input state.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Essentials

Handling input events

Receive controller input using either polling or callbacks.

protocol GCDevicePhysicalInput

The common properties and methods for objects that represent the input profile of a device.

protocol GCDevicePhysicalInputState

The common properties for physical devices with elements.

