

- Swift
- TaskGroup
-  TaskGroup.Element 

Type Alias

# TaskGroup.Element

The type of element produced by this asynchronous sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias Element = ChildTaskResult
```

Available when `ChildTaskResult` conforms to `Sendable`.

## See Also

### Supporting Types

struct Iterator

A type that provides an iteration interface over the results of tasks added to the group.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

