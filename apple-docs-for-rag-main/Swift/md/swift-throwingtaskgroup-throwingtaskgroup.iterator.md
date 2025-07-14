

- Swift
- ThrowingTaskGroup
-  ThrowingTaskGroup.Iterator 

Structure

# ThrowingTaskGroup.Iterator

A type that provides an iteration interface over the results of tasks added to the group.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Iterator
```

Available when `ChildTaskResult` conforms to `Sendable` and `Failure` conforms to `Error`.

## Overview

The elements returned by this iterator appear in the order that the tasks *completed*, not in the order that those tasks were added to the task group.

This iterator terminates after all tasks have completed successfully, or after any task completes by throwing an error. If a task completes by throwing an error, it doesn’t return any further task results. After iterating over the results of each task, it’s valid to make a new iterator for the task group, which you can use to iterate over the results of new tasks you add to the group. You can also make a new iterator to resume iteration after a child task throws an error. For example:

```
group.addTask { 1 }
group.addTask { throw SomeError }
group.addTask { 2 }

do {
    // Assuming the child tasks complete in order, this prints "1"
    // and then throws an error.
    for try await r in group { print(r) }
} catch {
    // Resolve the error.
}

// Assuming the child tasks complete in order, this prints "2".
for try await r in group { print(r) }
```

See Also

`ThrowingTaskGroup.next()`

## Topics

### Instance Methods

func cancel()

func next() async throws -> ThrowingTaskGroup&lt;ChildTaskResult, Failure>.Iterator.Element?

Advances to and returns the result of the next child task.

func next(isolation: isolated (any Actor)?) async throws(Failure) -> ThrowingTaskGroup&lt;ChildTaskResult, Failure>.Iterator.Element?

Advances to and returns the result of the next child task.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

## See Also

### Supporting Types

typealias Element

The type of element produced by this asynchronous sequence.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

