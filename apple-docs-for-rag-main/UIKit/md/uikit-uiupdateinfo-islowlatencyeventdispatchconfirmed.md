

- UIKit
- UIUpdateInfo
-  isLowLatencyEventDispatchConfirmed 

Instance Property

# isLowLatencyEventDispatchConfirmed

A Boolean value that indicates whether the system runs low-latency phases for the UI update.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var isLowLatencyEventDispatchConfirmed: Bool { get }
```

## Discussion

The value of this property is true when the system runs low-latency event dispatch during the UI update. Use this information to determine whether to avoid doing the same work more than once. For example, when considering whether to render a pencil-drawing stroke in afterEventDispatch, if this property is `true`, but isPerformingLowLatencyPhases is `false`, you might consider waiting until after low-latency event dispatch to render the stroke.

This value can change from `false` to `true` during the UI update, but not from `true` to `false`.

Important

Checking the value of this property can cause the system to commit to low-latency event dispatch unnecessarily. Check this property only when you have an intention to act on its value.

## See Also

### Working with low-latency updates

var isImmediatePresentationExpected: Bool

A Boolean value that indicates whether the system presents UI updates immediately upon completion.

var isPerformingLowLatencyPhases: Bool

A Boolean value that indicates whether the UI update is in the low-latency phases.

