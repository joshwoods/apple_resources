

- UIKit
- UIUpdateActionPhase
-  beforeLowLatencyEventDispatch 

Type Property

# beforeLowLatencyEventDispatch

A phase that runs before low-latency event handlers.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
class var beforeLowLatencyEventDispatch: UIUpdateActionPhase { get }
```

## Discussion

This phase runs before UIEvent and UIGestureRecognizer handlers run for low-latency eligible events.

This phase is off by default. You can request it to run by setting wantsLowLatencyEventDispatch to `true`.

## See Also

### Phases

class var afterUpdateScheduled: UIUpdateActionPhase

A phase that runs after the scheduling of a UI update.

class var beforeEventDispatch: UIUpdateActionPhase

A phase that runs before standard event handlers.

class var afterEventDispatch: UIUpdateActionPhase

A phase that runs after standard event handlers.

class var beforeCADisplayLinkDispatch: UIUpdateActionPhase

A phase that runs before Core Animation display link callbacks.

class var afterCADisplayLinkDispatch: UIUpdateActionPhase

A phase that runs after Core Animation display link callbacks.

class var beforeCATransactionCommit: UIUpdateActionPhase

A phase that runs before a Core Animation transaction commit.

class var afterCATransactionCommit: UIUpdateActionPhase

A phase that runs after a Core Animation transaction commit.

class var afterLowLatencyEventDispatch: UIUpdateActionPhase

A phase that runs after low-latency event handlers.

class var beforeLowLatencyCATransactionCommit: UIUpdateActionPhase

A phase that runs before a Core Animation transaction commit for a low-latency event.

class var afterLowLatencyCATransactionCommit: UIUpdateActionPhase

A phase that runs after a Core Animation transaction commit for a low-latency event.

class var afterUpdateComplete: UIUpdateActionPhase

A phase that runs at the end of a UI update.

