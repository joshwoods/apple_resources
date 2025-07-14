

- Foundation
- Progress
-  init(totalUnitCount:) 

Initializer

# init(totalUnitCount:)

Creates and returns a progress instance.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(totalUnitCount unitCount: Int64)
```

## Parameters 

`unitCount`  

The total number of units of work to assign to the progress instance.

## Discussion

If a current progress object exists, the initializer uses it to set the value of the totalUnitCount property.

In many cases, you can precede code that does a substantial amount of work with an invocation of this method, then repeatedly set the completedUnitCount or isCancelled property in the loop that does the work.

You can invoke this method on one thread and then message the returned Progress on another thread. For example, you can capture the created progress instance in a block that you pass to dispatch_async. In that block, you can invoke methods like becomeCurrent(withPendingUnitCount:) or resignCurrent(), and set the completedUnitCount or isCancelled properties as your app finishes its work.

## See Also

### Creating Progress Objects

init(parent: Progress?, userInfo: [ProgressUserInfoKey : Any]?)

Creates a new progress instance.

class func discreteProgress(totalUnitCount: Int64) -> Progress

Creates and returns a progress instance with the specified unit count that isn’t part of any existing progress tree.

init(totalUnitCount: Int64, parent: Progress, pendingUnitCount: Int64)

Creates a progress instance for the specified progress object with a unit count that’s a portion of the containing object’s total unit count.

