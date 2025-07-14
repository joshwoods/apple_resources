

- Swift
- Task
-  result 

Instance Property

# result

The result or error from a throwing task, after it completes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var result: Result { get async }
```

Available when `Success` conforms to `Sendable` and `Failure` conforms to `Error`.

## Return Value

If the task succeeded, `.success` with the task’s result as the associated value; otherwise, `.failure` with the error as the associated value.

## Discussion

If the task hasn’t completed, accessing this property waits for it to complete and its priority increases to that of the current task. Note that this might not be as effective as creating the task with the correct priority, depending on the executor’s scheduling details.

## See Also

### Accessing Results

var value: Success

The result from a throwing task, after it completes.

var value: Success

The result from a nonthrowing task, after it completes.

