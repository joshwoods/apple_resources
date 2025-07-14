

- Foundation
- Operation
-  isReady 

Instance Property

# isReady

A Boolean value indicating whether the operation can be performed now.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isReady: Bool { get }
```

## Discussion

The readiness of operations is determined by their dependencies on other operations and potentially by custom conditions that you define. The `NSOperation` class manages dependencies on other operations and reports the readiness of the receiver based on those dependencies.

If you want to use custom conditions to define the readiness of your operation object, reimplement this property and return a value that accurately reflects the readiness of the receiver. If you do so, your custom implementation must get the default property value from `super` and incorporate that readiness value into the new value of the property. In your custom implementation, you must generate KVO notifications for the `isReady` key path whenever the ready state of your operation object changes. For more information about generating KVO notifications, see Key-Value Observing Programming Guide.

## See Also

### Related Documentation

var dependencies: [Operation]

An array of the operation objects that must finish executing before the current object can begin executing.

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

var name: String?

The name of the operation.

