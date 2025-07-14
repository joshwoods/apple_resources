

- Foundation
- Progress
-  fractionCompleted 

Instance Property

# fractionCompleted

The fraction of the overall work that the progress object completes, including work from its suboperations.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var fractionCompleted: Double { get }
```

## Discussion

If the receiver object doesn’t have any suboperations, fractionCompleted is generally the result of dividing completedUnitCount by totalUnitCount. Setting both totalUnitCount and completedUnitCount properties to zero indicates that there is no progress to track. In this case, the isIndeterminate property returns false and the fractionCompleted property returns `0.0`.

If the receiver does have suboperations, fractionCompleted reflects progress from those progress objects in addition to its own completedUnitCount. When the suboperations finish, the completedUnitCount of the containing progress object updates.

## See Also

### Observing Progress

var isIndeterminate: Bool

A Boolean value that indicates whether the tracked progress is indeterminate.

var isFinished: Bool

A Boolean value that indicates the progress object is complete.

