

- Swift
- TaskGroup
-  waitForAll(isolation:) 

Instance Method

# waitForAll(isolation:)

Wait for all of the group’s remaining tasks to complete.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func waitForAll(isolation: isolated (any Actor)? = #isolation) async
```

## See Also

### Accessing Individual Results

func next(isolation: isolated (any Actor)?) async -> ChildTaskResult?

Wait for the next child task to complete, and return the value it returned.

var isEmpty: Bool

A Boolean value that indicates whether the group has any remaining tasks.

