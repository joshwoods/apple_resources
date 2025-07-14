

- OSLog
- OSLogStore
-  position(timeIntervalSinceLatestBoot:) 

Instance Method

# position(timeIntervalSinceLatestBoot:)

Returns a position representing time since the last boot in the series of entries.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func position(timeIntervalSinceLatestBoot seconds: TimeInterval) -> OSLogPosition
```

## See Also

### Accessing Position

func position(date: Date) -> OSLogPosition

Returns a position representing the time specified.

func position(timeIntervalSinceEnd: TimeInterval) -> OSLogPosition

Returns a position representing time since the end of the time range that the entries span.

