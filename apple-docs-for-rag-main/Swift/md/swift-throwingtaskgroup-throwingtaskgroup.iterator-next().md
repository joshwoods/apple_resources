

- Swift
- ThrowingTaskGroup
- ThrowingTaskGroup.Iterator
-  next() 

Instance Method

# next()

Advances to and returns the result of the next child task.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func next() async throws -> ThrowingTaskGroup.Iterator.Element?
```

## Return Value

The value returned by the next child task that completes, or `nil` if there are no remaining child tasks,

## Discussion

The elements returned from this method appear in the order that the tasks *completed*, not in the order that those tasks were added to the task group. After this method returns `nil`, this iterator is guaranteed to never produce more values.

For more information about the iteration order and semantics, see `ThrowingTaskGroup.next()`

Throws

The error thrown by the next child task that completes.

