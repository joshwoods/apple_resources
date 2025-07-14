

- Core Video
- CVTime
-  CVTime Values 

API Collection

# CVTime Values

Keys that represent Core Video time values.

## Topics

### Constants

let kCVZeroTime: CVTime

Zero time or duration. For example, CVDisplayLinkGetOutputVideoLatency(_:) returns `kCVZeroTime` for zero video latency.

let kCVIndefiniteTime: CVTime

An unknown or indefinite time. For example, CVDisplayLinkGetNominalOutputVideoRefreshPeriod(_:) returns `kCVIndefiniteTime` if the display link specified is not valid.

