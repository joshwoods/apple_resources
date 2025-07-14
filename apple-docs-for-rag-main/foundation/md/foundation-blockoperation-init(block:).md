

- Foundation
- BlockOperation
-  init(block:) 

Initializer

# init(block:)

Creates and returns an `NSBlockOperation` object and adds the specified block to it.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(block: @escaping () -> Void)
```

## Parameters 

`block`  

The block to add to the new block operation object’s list. The block should take no parameters and have no return value.

## Return Value

A new block operation object.

## See Also

### Related Documentation

Threading Programming Guide

### Managing the Blocks in the Operation

func addExecutionBlock(() -> Void)

Adds the specified block to the receiver’s list of blocks to perform.

var executionBlocks: [() -> Void]

The blocks associated with the receiver.

