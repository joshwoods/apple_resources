

- DockKit
- DockAccessory
-  DockAccessory.BatteryStates 

Structure

# DockAccessory.BatteryStates

An asynchronous sequence of dock accessory battery states.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
struct BatteryStates
```

## Topics

### Structures

struct Iterator

An object that allows iteration over dock accessory events.

### Instance Methods

func makeAsyncIterator() -> DockAccessory.BatteryStates.Iterator

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

