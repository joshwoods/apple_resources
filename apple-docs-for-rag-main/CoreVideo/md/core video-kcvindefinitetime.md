

- Core Video
-  kCVIndefiniteTime 

Global Variable

# kCVIndefiniteTime

An unknown or indefinite time. For example, CVDisplayLinkGetNominalOutputVideoRefreshPeriod(_:) returns `kCVIndefiniteTime` if the display link specified is not valid.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
let kCVIndefiniteTime: CVTime
```

## See Also

### Constants

let kCVZeroTime: CVTime

Zero time or duration. For example, CVDisplayLinkGetOutputVideoLatency(_:) returns `kCVZeroTime` for zero video latency.

