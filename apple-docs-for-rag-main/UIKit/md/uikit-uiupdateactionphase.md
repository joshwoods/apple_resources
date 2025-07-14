

- UIKit
-  UIUpdateActionPhase 

Class

# UIUpdateActionPhase

An object that defines specific phases of the UI update process.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
class UIUpdateActionPhase
```

## Overview

Each UI update consists of several phases that run in a consistent order, and the UIUpdateActionPhase object defines constants that represent these phases. When using a UIUpdateLink, you can use these constants to decide which phase of the UI update process you want its actions to run in.

There are two *phase groups*: standard and low-latency. The standard phase group runs for each UI update. This phase group includes these phases, which run in the following order:

1.  beforeEventDispatch

2.  afterEventDispatch

3.  beforeCADisplayLinkDispatch

4.  afterCADisplayLinkDispatch

5.  beforeCATransactionCommit

6.  afterCATransactionCommit

The low-latency phase group is optional, and it’s off by default. It runs only if you explicitly request low-latency event dispatch using wantsLowLatencyEventDispatch. The low-latency phase group includes these phases, which run in the following order (after the standard phases):

1.  beforeLowLatencyEventDispatch

2.  afterLowLatencyEventDispatch

3.  beforeLowLatencyCATransactionCommit

4.  afterLowLatencyCATransactionCommit

When a phase group runs, all phases inside the group run. Phases run one after another in the specified order without exiting back into the run loop.

## Topics

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

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### UI updates

class UIUpdateLink

An object you use to observe, participate in, and affect the UI update process.

class UIUpdateInfo

An object that contains detailed information about the current UI update state.

