

- Foundation
- Progress
-  current() 

Type Method

# current()

Returns the progress instance, if any.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func current() -> Progress?
```

## Return Value

The progress instance for the current thread, if any.

## Discussion

If you invoke becomeCurrent(withPendingUnitCount:) on the current thread, this method returns the progress instance.

Use this per-thread current() value to allow code that performs work to report useful progress even when it’s widely separated from the code that actually presents progress information to the user, and without requiring layers of intervening code to pass around an Progress instance.

To ensure that you report progress in known units of work, you typically work with a suboperation progress object that you create by calling discreteProgress(totalUnitCount:).

## See Also

### Accessing the Current Progress Object

func becomeCurrent(withPendingUnitCount: Int64)

Sets the progress object as the current object of the current thread, and assigns the amount of work for the next suboperation progress object to perform.

func addChild(Progress, withPendingUnitCount: Int64)

Adds a process object as a suboperation of a progress tree.

func performAsCurrent&lt;ReturnType>(withPendingUnitCount: Int64, using: () throws -> ReturnType) rethrows -> ReturnType

Retrieves the current thread’s progress object, executes the specified block, and increments the progress object by the specified units of work.

func resignCurrent()

Restores the previous progress object to become the current progress object on the thread.

