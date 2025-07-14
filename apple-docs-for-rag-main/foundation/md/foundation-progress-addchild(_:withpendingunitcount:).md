

- Foundation
- Progress
-  addChild(\_:withPendingUnitCount:) 

Instance Method

# addChild(\_:withPendingUnitCount:)

Adds a process object as a suboperation of a progress tree.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addChild(
    _ child: Progress,
    withPendingUnitCount inUnitCount: Int64
)
```

## Parameters 

`child`  

The progress instance to add to the progress tree.

`inUnitCount`  

The number of units of work for the new suboperation to complete.

## Discussion

You assign the suboperation a portion of the receiver’s total unit count according to `inUnitCount`. For more information, see Reporting Progress for Multiple Operations.

## See Also

### Accessing the Current Progress Object

class func current() -> Progress?

Returns the progress instance, if any.

func becomeCurrent(withPendingUnitCount: Int64)

Sets the progress object as the current object of the current thread, and assigns the amount of work for the next suboperation progress object to perform.

func performAsCurrent&lt;ReturnType>(withPendingUnitCount: Int64, using: () throws -> ReturnType) rethrows -> ReturnType

Retrieves the current thread’s progress object, executes the specified block, and increments the progress object by the specified units of work.

func resignCurrent()

Restores the previous progress object to become the current progress object on the thread.

