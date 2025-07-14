

- UIKit
- UIUpdateActionPhase
-  afterEventDispatch 

Type Property

# afterEventDispatch

A phase that runs after standard event handlers.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
class var afterEventDispatch: UIUpdateActionPhase { get }
```

## Discussion

This phase runs after UIEvent and UIGestureRecognizer handlers run for standard events. After that point, the app doesn’t receive new user input events. However, if you request low-latency event dispatch using wantsLowLatencyEventDispatch, more events might dispatch in the low-latency event dispatch phase.

Use this phase to perform tasks after processing all user input events for the UI update, like starting a parallel rendering thread.

## See Also

### Phases

class var afterUpdateScheduled: UIUpdateActionPhase

A phase that runs after the scheduling of a UI update.

class var beforeEventDispatch: UIUpdateActionPhase

A phase that runs before standard event handlers.

class var beforeCADisplayLinkDispatch: UIUpdateActionPhase

A phase that runs before Core Animation display link callbacks.

class var afterCADisplayLinkDispatch: UIUpdateActionPhase

A phase that runs after Core Animation display link callbacks.

class var beforeCATransactionCommit: UIUpdateActionPhase

A phase that runs before a Core Animation transaction commit.

class var afterCATransactionCommit: UIUpdateActionPhase

A phase that runs after a Core Animation transaction commit.

class var beforeLowLatencyEventDispatch: UIUpdateActionPhase

A phase that runs before low-latency event handlers.

class var afterLowLatencyEventDispatch: UIUpdateActionPhase

A phase that runs after low-latency event handlers.

class var beforeLowLatencyCATransactionCommit: UIUpdateActionPhase

A phase that runs before a Core Animation transaction commit for a low-latency event.

class var afterLowLatencyCATransactionCommit: UIUpdateActionPhase

A phase that runs after a Core Animation transaction commit for a low-latency event.

class var afterUpdateComplete: UIUpdateActionPhase

A phase that runs at the end of a UI update.

