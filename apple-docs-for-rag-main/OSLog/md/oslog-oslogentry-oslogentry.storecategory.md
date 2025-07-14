

- OSLog
- OSLogEntry
-  OSLogEntry.StoreCategory 

Enumeration

# OSLogEntry.StoreCategory

A classification of how the entry was to be stored and rotated at the point when it was created.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum StoreCategory
```

## Overview

The unified logging system keeps entries in one of two locations: a ring buffer in memory, or a persisted data store. Entries rotate out to free up resources; they are rotated out in bulk according to heuristics based on space, time, and entry classification.

## Topics

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

case longTerm3

The entry was tagged with a hint indicating the system should try to preserve it for approximately 3 days.

case longTerm7

The entry was tagged with a hint indicating the system should try to preserve it for approximately 7 days.

case longTerm14

The entry was tagged with a hint indicating the system should try to preserve it for approximately 14 days.

case longTerm30

The entry was tagged with a hint indicating the system should try to preserve it for approximately 30 days.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Store Categories

var storeCategory: OSLogEntry.StoreCategory

The current log entry’s storage tag.

