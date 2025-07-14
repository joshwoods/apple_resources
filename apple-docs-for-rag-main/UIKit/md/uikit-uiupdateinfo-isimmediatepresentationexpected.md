

- UIKit
- UIUpdateInfo
-  isImmediatePresentationExpected 

Instance Property

# isImmediatePresentationExpected

A Boolean value that indicates whether the system presents UI updates immediately upon completion.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var isImmediatePresentationExpected: Bool { get }
```

## Discussion

The value of this property is true when the system presents UI updates immediately upon completion. Use this information to determine whether to minimize the complexity of the code you run during the UI update. Defer any processing that isn’t critical for the current UI update until after the UI update finishes.

This value can change during the UI update.

## See Also

### Working with low-latency updates

var isLowLatencyEventDispatchConfirmed: Bool

A Boolean value that indicates whether the system runs low-latency phases for the UI update.

var isPerformingLowLatencyPhases: Bool

A Boolean value that indicates whether the UI update is in the low-latency phases.

