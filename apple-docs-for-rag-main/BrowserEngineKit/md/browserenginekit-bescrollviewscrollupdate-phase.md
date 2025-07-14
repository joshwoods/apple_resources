

- BrowserEngineKit
- BEScrollViewScrollUpdate
-  phase 

Instance Property

# phase

The point in the scrolling lifecycle represented by the scroll update.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
var phase: BEScrollViewScrollUpdate.Phase { get }
```

## Overview

The phases of a scroll update represent a state machine:

1.  A scroll gesture is initially in the BEScrollViewScrollUpdate.Phase.began phase, when the person puts their finger down in the scroll view.

2.  As the person interacts with the scroll view, the system generates zero or more BEScrollViewScrollUpdate.Phase.changed updates for the scroll gesture.

3.  Finally, the scroll gesture either enters the BEScrollViewScrollUpdate.Phase.ended phase when the person stops interacting with the scroll view; or it becomes BEScrollViewScrollUpdate.Phase.cancelled when the operating system receives another event that means it stops tracking the scroll gesture.

## See Also

### Retrieving scroll state information

var timestamp: TimeInterval

The time at which the scroll update occurred.

enum Phase

The phase of a scroll update in a scroll gesture’s lifecycle.

