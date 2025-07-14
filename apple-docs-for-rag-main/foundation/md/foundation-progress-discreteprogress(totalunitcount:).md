

- Foundation
- Progress
-  discreteProgress(totalUnitCount:) 

Type Method

# discreteProgress(totalUnitCount:)

Creates and returns a progress instance with the specified unit count that isn’t part of any existing progress tree.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func discreteProgress(totalUnitCount unitCount: Int64) -> Progress
```

## Parameters 

`unitCount`  

The total number of units of work to assign to the progress instance.

## Return Value

A new progress instance with its containing progress object set to `nil.`

## Discussion

Use this method to create the top-level progress object that your custom classes return. The receiver of the returned progress object can add it to a progress tree using addChild(_:withPendingUnitCount:).

You’re responsible for updating the progress count of the created progress object. You can invoke this method on one thread and then message the returned `NSProgress` on another thread. For example, you can capture the created progress instance in a block that you pass to dispatch_async. In that block, you can invoke methods like becomeCurrent(withPendingUnitCount:) or resignCurrent(), and set the completedUnitCount or isCancelled properties as your app finishes its work.

## See Also

### Creating Progress Objects

init(parent: Progress?, userInfo: [ProgressUserInfoKey : Any]?)

Creates a new progress instance.

init(totalUnitCount: Int64)

Creates and returns a progress instance.

init(totalUnitCount: Int64, parent: Progress, pendingUnitCount: Int64)

Creates a progress instance for the specified progress object with a unit count that’s a portion of the containing object’s total unit count.

