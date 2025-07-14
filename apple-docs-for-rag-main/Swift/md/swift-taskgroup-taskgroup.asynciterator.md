

- Swift
- TaskGroup
-  TaskGroup.AsyncIterator 

Type Alias

# TaskGroup.AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias AsyncIterator = TaskGroup.Iterator
```

Available when `ChildTaskResult` conforms to `Sendable`.

## See Also

### Supporting Types

typealias Element

The type of element produced by this asynchronous sequence.

struct Iterator

A type that provides an iteration interface over the results of tasks added to the group.

