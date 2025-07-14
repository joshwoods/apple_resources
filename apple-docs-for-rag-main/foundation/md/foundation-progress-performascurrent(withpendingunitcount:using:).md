

- Foundation
- Progress
-  performAsCurrent(withPendingUnitCount:using:) 

Instance Method

# performAsCurrent(withPendingUnitCount:using:)

Retrieves the current thread’s progress object, executes the specified block, and increments the progress object by the specified units of work.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func performAsCurrent(
    withPendingUnitCount unitCount: Int64,
    using work: () throws -> ReturnType
) rethrows -> ReturnType
```

## Parameters 

`unitCount`  

The number of units of work to increment for the current progress object. This number represents the portion of work that is complete in relation to the total number of units of work for the current thread’s progress object. The units of work for this parameter must be the same units of work as the current progress object’s totalUnitCount property.

`work`  

A block that wraps the work you specify to complete for incrementing the current progress.

## Return Value

The return type and value of the block that you specify for the `work` parameter.

## Discussion

Use this function as a convenience method to wrap an existing method or block to increment the current progress object. This function retrieves the current progress object, does the work you specify in the work block, and returns the value from that block. When the block is complete, this function increments the current progress object. This function is the same as calling becomeCurrent(withPendingUnitCount:), doing the work you specify in the block, and calling resignCurrent().

## See Also

### Accessing the Current Progress Object

class func current() -> Progress?

Returns the progress instance, if any.

func becomeCurrent(withPendingUnitCount: Int64)

Sets the progress object as the current object of the current thread, and assigns the amount of work for the next suboperation progress object to perform.

func addChild(Progress, withPendingUnitCount: Int64)

Adds a process object as a suboperation of a progress tree.

func resignCurrent()

Restores the previous progress object to become the current progress object on the thread.

