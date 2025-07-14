

- Foundation
- Progress
-  init(parent:userInfo:) 

Initializer

# init(parent:userInfo:)

Creates a new progress instance.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    parent parentProgressOrNil: Progress?,
    userInfo userInfoOrNil: [ProgressUserInfoKey : Any]? = nil
)
```

## Parameters 

`parentProgressOrNil`  

The containing Progress object, if any, to notify when reporting progress, or to consult when checking for cancellation.

The only valid values are current() or `nil`.

`userInfoOrNil`  

The optional user information dictionary for the progress object.

## Discussion

This is the designated initializer for the Progress class.

## See Also

### Creating Progress Objects

class func discreteProgress(totalUnitCount: Int64) -> Progress

Creates and returns a progress instance with the specified unit count that isn’t part of any existing progress tree.

init(totalUnitCount: Int64)

Creates and returns a progress instance.

init(totalUnitCount: Int64, parent: Progress, pendingUnitCount: Int64)

Creates a progress instance for the specified progress object with a unit count that’s a portion of the containing object’s total unit count.

