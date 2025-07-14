

- Foundation
- Progress
-  isFinished 

Instance Property

# isFinished

A Boolean value that indicates the progress object is complete.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isFinished: Bool { get }
```

## Discussion

A progress object finishes when the completedUnitCount equals or exceeds the totalUnitCount.

By default, Progress is KVO-compliant for this property. It sends notifications on the same thread that updates the property.

## See Also

### Observing Progress

var isIndeterminate: Bool

A Boolean value that indicates whether the tracked progress is indeterminate.

var fractionCompleted: Double

The fraction of the overall work that the progress object completes, including work from its suboperations.

