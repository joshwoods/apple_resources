

- BrowserEngineKit
- BEScrollViewScrollUpdate
-  timestamp 

Instance Property

# timestamp

The time at which the scroll update occurred.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
var timestamp: TimeInterval { get }
```

## See Also

### Retrieving scroll state information

var phase: BEScrollViewScrollUpdate.Phase

The point in the scrolling lifecycle represented by the scroll update.

enum Phase

The phase of a scroll update in a scroll gesture’s lifecycle.

