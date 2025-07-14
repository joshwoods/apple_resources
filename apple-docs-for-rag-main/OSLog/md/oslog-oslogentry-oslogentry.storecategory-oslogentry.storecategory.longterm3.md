

- OSLog
- OSLogEntry
- OSLogEntry.StoreCategory
-  OSLogEntry.StoreCategory.longTerm3 

Case

# OSLogEntry.StoreCategory.longTerm3

The entry was tagged with a hint indicating the system should try to preserve it for approximately 3 days.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case longTerm3
```

## Discussion

It was persisted in the filesystem-backed date store, and rotation of these entries was based on both time and space considerations.

## See Also

### Constants

case undefined

This entry’s purpose is unknown.

case metadata

This entry was generated as information about the other entries or about the sequence of entries as a whole.

case shortTerm

This entry was not intended to be long-lived, and was captured in the ring buffer.

case longTermAuto

The entry was tagged with a hint indicating the system should try to preserve it based on the amount of space available.

case longTerm1

The entry was tagged with a hint indicating the system should try to preserve it for approximately 1 day.

case longTerm7

The entry was tagged with a hint indicating the system should try to preserve it for approximately 7 days.

case longTerm14

The entry was tagged with a hint indicating the system should try to preserve it for approximately 14 days.

case longTerm30

The entry was tagged with a hint indicating the system should try to preserve it for approximately 30 days.

