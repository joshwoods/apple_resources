

- Foundation
- Operation
-  name 

Instance Property

# name

The name of the operation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var name: String? { get set }
```

## Discussion

Assign a name to the operation object to help identify it during debugging.

## See Also

### Getting the Operation Status

var isCancelled: Bool

A Boolean value indicating whether the operation has been cancelled

var isExecuting: Bool

A Boolean value indicating whether the operation is currently executing.

var isFinished: Bool

A Boolean value indicating whether the operation has finished executing its task.

var isConcurrent: Bool

A Boolean value indicating whether the operation executes its task asynchronously.

var isAsynchronous: Bool

A Boolean value indicating whether the operation executes its task asynchronously.

var isReady: Bool

A Boolean value indicating whether the operation can be performed now.

