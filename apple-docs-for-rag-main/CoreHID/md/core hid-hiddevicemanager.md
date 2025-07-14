

- Core HID
-  HIDDeviceManager 

Class

# HIDDeviceManager

A helper for discovering human interface devices (HID) connected to the system.

macOS 15.0+

``` source
actor HIDDeviceManager
```

## Mentioned in 

Communicating with human interface devices

## Overview

Use this class to specify matching criteria to filter all of the discoverable devices connected to the system into devices of interest. This is the main method of receiving a HIDDeviceClient.DeviceReference used to create a HIDDeviceClient.

Matching criteria are specified by creating HIDDeviceManager.DeviceMatchingCriteria and passing them to monitorNotifications(matchingCriteria:). References to devices that match the criteria are received using HIDDeviceManager.Notification.deviceMatched(_:) notifications.

## Topics

### Create a device manager

init()

Creates a matching service for HID devices.

### Monitor device notifications

func monitorNotifications(matchingCriteria: [HIDDeviceManager.DeviceMatchingCriteria]) -> AsyncThrowingStream&lt;HIDDeviceManager.Notification, any Error>

Creates an asynchronous stream that receives notifications for devices of interest.

enum Notification

Notifications for HID devices.

### Structures

struct DeviceMatchingCriteria

Matching criteria used to filter HID devices.

### Instance Properties

var unownedExecutor: UnownedSerialExecutor

Retrieve the executor for this actor as an optimized, unowned reference.

### Default Implementations

Actor Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Actor
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Discovery

Discovering HID devices from Terminal

Identify devices connected to your Mac from the command line.

struct DeviceMatchingCriteria

Matching criteria used to filter HID devices.

