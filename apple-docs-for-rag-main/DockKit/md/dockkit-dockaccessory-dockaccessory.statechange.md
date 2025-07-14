

- DockKit
- DockAccessory
-  DockAccessory.StateChange 

Structure

# DockAccessory.StateChange

An event that indicates a change in the state of a dock accessory.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct StateChange
```

## Overview

DockKit generates this event when a device docks or undocks from the dock accessory, or when a person presses the tracking button. To iterate the stream of state changes, see accessoryStateChanges.

## Topics

### Getting properties

let accessory: DockAccessory?

The dock accessory that generated the event.

let state: DockAccessory.State

The state of the dock accessory associated with the event.

### Instance Properties

let trackingButtonEnabled: Bool

The state of the tracking button on the dock accessory.

## Relationships

### Conforms To

- Sendable

## See Also

### Getting accessory information

var firmwareVersion: String?

The firmware version of the dock accessory.

var hardwareModel: String?

The model of the dock accessory.

let identifier: DockAccessory.Identifier

The name and unique identifer of the dock accessory.

struct Identifier

Information that uniquely identifies the dock accessory.

enum Category

Types of supported dock accesories.

enum State

The state of a dock accessory.

struct StateChanges

An asynchronous sequence of dock accessory state changes.

