

- DockKit
- DockAccessory
-  DockAccessory.AccessoryEvents 

Structure

# DockAccessory.AccessoryEvents

An asynchronous sequence of dock accessory events.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+

``` source
struct AccessoryEvents
```

## Topics

### Structures

struct Iterator

An object that allows iteration over dock accessory events.

### Instance Methods

func makeAsyncIterator() -> DockAccessory.AccessoryEvents.Iterator

Creates and returns an iterator that traverses the list of dock accessory events.

### Type Aliases

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

A dock accessory event.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

