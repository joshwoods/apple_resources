

- DockKit
-  DockAccessoryManager 

Class

# DockAccessoryManager

Observe the state of dock accessories and enable or disable system tracking.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
class DockAccessoryManager
```

## Overview

`DockAccessoryManager` enables and disables system tracking for camera-enabled apps, and provides docking and undocking notifications. If you want to customize the tracking behavior of a dock accessory, use accessoryStateChanges to obtain that accessory.

This class is a singleton, so use shared to fetch the single instance.

## Topics

### Obtaining a manager

static let shared: DockAccessoryManager

The accessory manager singleton object.

### Controlling dock accessories

var accessoryStateChanges: DockAccessory.StateChanges

Obtain a reference to a dock accessory and receive notifications about its state.

### Changing tracking behavior

var isSystemTrackingEnabled: Bool

An indication of whether system tracking is enabled.

func setSystemTrackingEnabled(Bool) async throws

Enable and disable system tracking for camera-enabled apps.

## Relationships

### Conforms To

- Sendable

## See Also

### Controlling the dock accessory

Controlling a DockKit accessory using your camera app

Follow subjects in real time using an iPhone that you mount on a DockKit accessory.

class DockAccessory

Obtain accessory information and control tracking behavior.

enum DockKitError

A list of errors that DockKit sends.

