

- DockKit
- DockAccessory
- DockAccessory.TrackingStates
-  DockAccessory.TrackingStates.Iterator 

Structure

# DockAccessory.TrackingStates.Iterator

An object that allows iteration over tracking states.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() async -> DockAccessory.TrackingState?

Provide the next tracking session state in the list.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

