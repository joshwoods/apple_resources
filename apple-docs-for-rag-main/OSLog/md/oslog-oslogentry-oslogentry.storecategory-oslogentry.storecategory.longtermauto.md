

- OSLog
- OSLogEntry
- OSLogEntry.StoreCategory
-  OSLogEntry.StoreCategory.longTermAuto 

Case

# OSLogEntry.StoreCategory.longTermAuto

The entry was tagged with a hint indicating the system should try to preserve it based on the amount of space available.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case longTermAuto
```

## Discussion

Instead of tagging a hint with a number of days that the entry should be preserved, the `longTermAuto` case is preserved based on the amount of space available. Therefore, it will automatically make determinations on how long to preserve the entry. Entries using this case should be persisted in a filesystem-backed data store.

## See Also

### Constants

case undefined

This entry’s purpose is unknown.

case metadata

This entry was generated as information about the other entries or about the sequence of entries as a whole.

case shortTerm

This entry was not intended to be long-lived, and was captured in the ring buffer.

case longTerm1

The entry was tagged with a hint indicating the system should try to preserve it for approximately 1 day.

case longTerm3

The entry was tagged with a hint indicating the system should try to preserve it for approximately 3 days.

case longTerm7

The entry was tagged with a hint indicating the system should try to preserve it for approximately 7 days.

case longTerm14

The entry was tagged with a hint indicating the system should try to preserve it for approximately 14 days.

case longTerm30

The entry was tagged with a hint indicating the system should try to preserve it for approximately 30 days.

