

- Foundation
- Operation
-  removeDependency(\_:) 

Instance Method

# removeDependency(\_:)

Removes the receiver’s dependence on the specified operation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeDependency(_ op: Operation)
```

## Parameters 

`op`  

The dependent operation to be removed from the receiver.

## Discussion

This method may change the `isReady` and `dependencies` properties of the receiver.

## See Also

### Managing Dependencies

func addDependency(Operation)

Makes the receiver dependent on the completion of the specified operation.

var dependencies: [Operation]

An array of the operation objects that must finish executing before the current object can begin executing.

