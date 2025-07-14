

- DockKit
- DockAccessory
- DockAccessory.MotionStates
-  DockAccessory.MotionStates.Iterator 

Structure

# DockAccessory.MotionStates.Iterator

An object that allows iteration over dock accessory motion states.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() async -> DockAccessory.MotionState?

Provide the next dock accessory motion state in the list.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

## See Also

### Iterating over motion states

func makeAsyncIterator() -> DockAccessory.MotionStates.Iterator

Creates and returns an iterator that traverses the list of dock accessory motion states.

typealias Element

A dock accessory motion state.

