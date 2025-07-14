

- DockKit
- DockAccessory
- DockAccessory.StateChanges
-  DockAccessory.StateChanges.Iterator 

Structure

# DockAccessory.StateChanges.Iterator

An object that allows iteration over dock accessory state changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct Iterator
```

## Topics

### Iterating over state changes

func next() async -> DockAccessory.StateChange?

Provide the next dock accessory state change in the list.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

## See Also

### Iterating over state changes

func makeAsyncIterator() -> DockAccessory.StateChanges.Iterator

Creates and returns an iterator that traverses the list of dock accessory state changes.

typealias Element

A dock accessory state change.

