

- DockKit
- DockAccessory
- DockAccessory.BatteryStates
-  DockAccessory.BatteryStates.Iterator 

Structure

# DockAccessory.BatteryStates.Iterator

An object that allows iteration over dock accessory events.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() async -> DockAccessory.BatteryState?

Provide the next dock accessory event in the list.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

