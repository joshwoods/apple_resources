

- DockKit
- DockAccessory
-  DockAccessory.MotionStates 

Structure

# DockAccessory.MotionStates

An asynchronous sequence of orientation and velocity updates from the device.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct MotionStates
```

## Topics

### Iterating over motion states

struct Iterator

An object that allows iteration over dock accessory motion states.

func makeAsyncIterator() -> DockAccessory.MotionStates.Iterator

Creates and returns an iterator that traverses the list of dock accessory motion states.

typealias Element

A dock accessory motion state.

### Type Aliases

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Getting position and limits

var motionStates: DockAccessory.MotionStates

Motion information from the dock accessory that includes current orientation and velocity of all axes.

var limits: DockAccessory.Limits

Current limits for the axes of rotation and maximum angular velocity.

struct MotionState

An event that indicates the state of a dock accessory’s current position and speed.

struct Limits

Soft limits on multiple axes of rotation.

