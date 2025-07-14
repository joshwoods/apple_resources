

- DockKit
- DockAccessory
- DockAccessory.AccessoryEvents
-  DockAccessory.AccessoryEvents.Iterator 

Structure

# DockAccessory.AccessoryEvents.Iterator

An object that allows iteration over dock accessory events.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() async -> DockAccessory.AccessoryEvent?

Provide the next dock accessory event in the list.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

