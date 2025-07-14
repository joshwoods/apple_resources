

- Foundation
- Operation
-  addDependency(\_:) 

Instance Method

# addDependency(\_:)

Makes the receiver dependent on the completion of the specified operation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addDependency(_ op: Operation)
```

## Parameters 

`op`  

The operation on which the receiver should depend. The same dependency should not be added more than once to the receiver, and the results of doing so are undefined.

## Discussion

The receiver is not considered ready to execute until all of its dependent operations have finished executing. If the receiver is already executing its task, adding dependencies has no practical effect. This method may change the `isReady` and `dependencies` properties of the receiver.

It is a programmer error to create any circular dependencies among a set of operations. Doing so can cause a deadlock among the operations and may freeze your program.

## See Also

### Managing Dependencies

func removeDependency(Operation)

Removes the receiver’s dependence on the specified operation.

var dependencies: [Operation]

An array of the operation objects that must finish executing before the current object can begin executing.

