

- UIKit
- UIUpdateInfo
-  isPerformingLowLatencyPhases 

Instance Property

# isPerformingLowLatencyPhases

A Boolean value that indicates whether the UI update is in the low-latency phases.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var isPerformingLowLatencyPhases: Bool { get }
```

## Discussion

The value of this property is true between the beforeLowLatencyEventDispatch and afterLowLatencyCATransactionCommit UI update phases. Keep any code you run in this part of the UI update as minimal as possible, especially when isImmediatePresentationExpected is `true`. Defer any processing that isn’t critical for the current UI update until afterLowLatencyCATransactionCommit.

## See Also

### Working with low-latency updates

var isImmediatePresentationExpected: Bool

A Boolean value that indicates whether the system presents UI updates immediately upon completion.

var isLowLatencyEventDispatchConfirmed: Bool

A Boolean value that indicates whether the system runs low-latency phases for the UI update.

