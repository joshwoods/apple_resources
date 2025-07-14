

- Foundation
- Progress
-  becomeCurrent(withPendingUnitCount:) 

Instance Method

# becomeCurrent(withPendingUnitCount:)

Sets the progress object as the current object of the current thread, and assigns the amount of work for the next suboperation progress object to perform.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func becomeCurrent(withPendingUnitCount unitCount: Int64)
```

## Parameters 

`unitCount`  

The number of units of work for the next progress object that initializes when you invoke init(parent:userInfo:) in the current thread with this progress object as the containing progress object.

The number represents the portion of work to perform in relation to the total number of units of work, which is the value of the progress object’s totalUnitCount property. The units of work for this parameter must be the same units of work in the progress object’s totalUnitCount property.

## Discussion

Use this method to build a tree of progress objects, as Reporting Progress for Multiple Operations describes.

## See Also

### Accessing the Current Progress Object

class func current() -> Progress?

Returns the progress instance, if any.

func addChild(Progress, withPendingUnitCount: Int64)

Adds a process object as a suboperation of a progress tree.

func performAsCurrent&lt;ReturnType>(withPendingUnitCount: Int64, using: () throws -> ReturnType) rethrows -> ReturnType

Retrieves the current thread’s progress object, executes the specified block, and increments the progress object by the specified units of work.

func resignCurrent()

Restores the previous progress object to become the current progress object on the thread.

