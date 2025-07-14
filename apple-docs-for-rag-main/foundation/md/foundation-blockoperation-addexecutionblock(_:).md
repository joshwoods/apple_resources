

- Foundation
- BlockOperation
-  addExecutionBlock(\_:) 

Instance Method

# addExecutionBlock(\_:)

Adds the specified block to the receiver’s list of blocks to perform.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addExecutionBlock(_ block: @escaping () -> Void)
```

## Parameters 

`block`  

The block to add to the receiver’s list. The block should take no parameters and have no return value.

## Discussion

The specified block should not make any assumptions about its execution environment.

Calling this method while the receiver is executing or has already finished causes an `NSInvalidArgumentException` exception to be thrown.

## See Also

### Managing the Blocks in the Operation

convenience init(block: () -> Void)

Creates and returns an `NSBlockOperation` object and adds the specified block to it.

var executionBlocks: [() -> Void]

The blocks associated with the receiver.

