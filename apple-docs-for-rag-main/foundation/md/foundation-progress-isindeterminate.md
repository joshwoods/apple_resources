

- Foundation
- Progress
-  isIndeterminate 

Instance Property

# isIndeterminate

A Boolean value that indicates whether the tracked progress is indeterminate.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isIndeterminate: Bool { get }
```

## Discussion

Use isIndeterminate progress only when you’re unable to determine a reasonable value for either completedUnitCount or totalUnitCount. Progress is indeterminate when the value of the totalUnitCount or completedUnitCount is less than zero or if both values are zero. When progress is indeterminate, fractionCompleted returns `0.0` and isFinished returns `false`.

By default, Progress is KVO-compliant for this property. It sends notifications on the same thread that updates the property.

The following code snippet clarifies the behavior for setting both totalUnitCount and completedUnitCount to `0`.

```
let progress = Progress(totalUnitCount: 0) 
progress.completedUnitCount = 0 // default 
print("totalUnitCount: (progress.totalUnitCount)") 
print("completedUnitCount: (progress.completedUnitCount)") 
print("isIndeterminate: (progress.isIndeterminate)") 
print("fractionCompleted: (progress.fractionCompleted)") 
print("isFinished: (progress.isFinished)")
/*
Code Output:
totalUnitCount: 0 completedUnitCount: 0 isIndeterminate: true fractionCompleted: 0.0 isFinished: false
*/
```

## See Also

### Observing Progress

var fractionCompleted: Double

The fraction of the overall work that the progress object completes, including work from its suboperations.

var isFinished: Bool

A Boolean value that indicates the progress object is complete.

