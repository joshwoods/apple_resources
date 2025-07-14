

- Core Media
-  CMBufferQueue 

Class

# CMBufferQueue

A reference to a buffer queue instance.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
class CMBufferQueue
```

## Overview

A `CMBufferQueue` is a queue of timed buffers backed by a Core Foundation object.

## Topics

### Managing a Queue

func enqueue(CMBuffer) throws

Enqueues a buffer to the queue.

func dequeue() -> CMBuffer?

Dequeues a buffer from the queue.

func dequeueIfDataReady() -> CMBuffer?

Dequeues a buffer from the queue, if it’s ready.

func markEndOfData() throws

Marks a buffer as being at the end of its data.

func reset() throws

Empties the queue and resets its end-of-data state.

func reset((CMBuffer) throws -> ()) throws

Resets a buffer with a callback block.

### Managing Triggers

func installTrigger(condition: CMBufferQueue.TriggerCondition, CMBufferQueueTriggerHandler?) throws -> CMBufferQueue.TriggerToken

Installs a trigger on the queue.

func removeTrigger(CMBufferQueue.TriggerToken) throws

Removes a trigger from the queue.

func testTrigger(CMBufferQueue.TriggerToken) -> Bool

Tests a trigger condition.

typealias TriggerToken

A type alias for a trigger token.

enum TriggerCondition

An enumeration of trigger conditions.

### Inspecting Duration and Timing

var duration: CMTime

The sum of all durations of buffers in the queue.

var totalSize: Int

The total size of all buffers in the queue.

var firstDecodeTimeStamp: CMTime

The decode timestamp of the first buffer in the queue.

var firstPresentationTimeStamp: CMTime

The presentation timestamp of the first buffer in the queue.

var endPresentationTimeStamp: CMTime

The greatest end presentation timestamp.

var minDecodeTimeStamp: CMTime

The earliest decode timestamp.

var minPresentationTimeStamp: CMTime

The earliest presentation timestamp.

var maxPresentationTimeStamp: CMTime

The greatest presentation timestamp.

### Inspecting a Queue

var isEmpty: Bool

A Boolean value that indicates whether the queue contains buffers.

var bufferCount: CMItemCount

The count of buffers in the queue.

var head: CMBuffer?

The element at the head of the queue.

var containsEndOfData: Bool

A Boolean value that indicates whether the buffer has its end-of-data state set.

var isAtEndOfData: Bool

A Boolean value that indicates whether that queue is at the end of its data.

### Validating a Queue

func setValidationHandler((CMBufferQueue, CMBuffer) throws -> Void)

Sets validation handler for the queue to call before enqueuing buffers.

### Accessing Buffers

var buffers: CMBufferQueue.Buffers

The buffers that the queue contains.

### Accessing the Type Identifier

class var typeID: CFTypeID

The type identifier for this object.

### Data Types

struct Buffers

struct Handlers

struct Error

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

