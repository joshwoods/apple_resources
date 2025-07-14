

- Swift
- ThrowingTaskGroup
-  next() 

Instance Method

# next()

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func next() async throws -> ChildTaskResult?
```

## See Also

### Accessing Individual Results

func nextResult(isolation: isolated (any Actor)?) async -> Result&lt;ChildTaskResult, Failure>?

Wait for the next child task to complete, and return a result containing either the value that the child task returned or the error that it threw.

var isEmpty: Bool

A Boolean value that indicates whether the group has any remaining tasks.

func waitForAll(isolation: isolated (any Actor)?) async throws

Wait for all of the group’s remaining tasks to complete.

