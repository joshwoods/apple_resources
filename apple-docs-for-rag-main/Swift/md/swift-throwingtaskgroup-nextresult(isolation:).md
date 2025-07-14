

- Swift
- ThrowingTaskGroup
-  nextResult(isolation:) 

Instance Method

# nextResult(isolation:)

Wait for the next child task to complete, and return a result containing either the value that the child task returned or the error that it threw.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func nextResult(isolation: isolated (any Actor)? = #isolation) async -> Result?
```

## Return Value

A `Result.success` value containing the value that the child task returned, or a `Result.failure` value containing the error that the child task threw.

## Discussion

The values returned by successive calls to this method appear in the order that the tasks *completed*, not in the order that those tasks were added to the task group. For example:

```
group.addTask { 1 }
group.addTask { 2 }

guard let result = await group.nextResult() else {
    return  // No task to wait on, which won't happen in this example.
}

switch result {
case .success(let value): print(value)
case .failure(let error): print("Failure: \(error)")
}
// Prints either "2" or "1".
```

If the next child task throws an error and you propagate that error from this method out of the body of a call to the `ThrowingTaskGroup.withThrowingTaskGroup(of:returning:body:)` method, then all remaining child tasks in that group are implicitly canceled.

See Also

`next()`

## See Also

### Accessing Individual Results

func next() async throws -> ChildTaskResult?

var isEmpty: Bool

A Boolean value that indicates whether the group has any remaining tasks.

func waitForAll(isolation: isolated (any Actor)?) async throws

Wait for all of the group’s remaining tasks to complete.

