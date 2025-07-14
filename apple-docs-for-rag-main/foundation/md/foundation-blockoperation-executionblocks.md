

- Foundation
- BlockOperation
-  executionBlocks 

Instance Property

# executionBlocks

The blocks associated with the receiver.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var executionBlocks: [() -> Void] { get }
```

## Discussion

The blocks in this array are copies of those originally added using the addExecutionBlock(_:) method.

## See Also

### Managing the Blocks in the Operation

convenience init(block: () -> Void)

Creates and returns an `NSBlockOperation` object and adds the specified block to it.

func addExecutionBlock(() -> Void)

Adds the specified block to the receiver’s list of blocks to perform.

