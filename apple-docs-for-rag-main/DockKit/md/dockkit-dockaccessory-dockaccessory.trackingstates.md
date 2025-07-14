

- DockKit
- DockAccessory
-  DockAccessory.TrackingStates 

Structure

# DockAccessory.TrackingStates

An asynchronous sequence of tracking session states.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
struct TrackingStates
```

## Topics

### Structures

struct Iterator

An object that allows iteration over tracking states.

### Instance Methods

func makeAsyncIterator() -> DockAccessory.TrackingStates.Iterator

Create and return an iterator that traverses the list of tracking session states.

### Type Aliases

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

A tracking session state.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

