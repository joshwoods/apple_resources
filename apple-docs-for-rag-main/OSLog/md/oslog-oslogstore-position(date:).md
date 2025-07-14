

- OSLog
- OSLogStore
-  position(date:) 

Instance Method

# position(date:)

Returns a position representing the time specified.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func position(date: Date) -> OSLogPosition
```

## Discussion

If there are multiple occurrences of the same time, the method returns the earliest occurrence.

## See Also

### Accessing Position

func position(timeIntervalSinceEnd: TimeInterval) -> OSLogPosition

Returns a position representing time since the end of the time range that the entries span.

func position(timeIntervalSinceLatestBoot: TimeInterval) -> OSLogPosition

Returns a position representing time since the last boot in the series of entries.

