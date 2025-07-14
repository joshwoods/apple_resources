

- DockKit
- DockAccessory
-  DockAccessory.StateChanges 

Structure

# DockAccessory.StateChanges

An asynchronous sequence of dock accessory state changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct StateChanges
```

## Topics

### Iterating over state changes

struct Iterator

An object that allows iteration over dock accessory state changes.

func makeAsyncIterator() -> DockAccessory.StateChanges.Iterator

Creates and returns an iterator that traverses the list of dock accessory state changes.

typealias Element

A dock accessory state change.

### Type Aliases

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

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

struct StateChange

An event that indicates a change in the state of a dock accessory.

