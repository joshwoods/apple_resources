

- OSLog
-  OSLogStore 

Class

# OSLogStore

A set of entries from the unified logging system.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class OSLogStore
```

## Overview

Instances of this class represent a fixed range of entries and may be backed by a `logarchive` or your Mac’s local store.

In Swift, Use the getEntries(with:at:matching:) function to retrieve a filtered array of log entries.

In Objective-C, use instances of this class to create OSLogEnumerator objects. One store can support multiple `OSLogEnumerator` instances concurrently.

## Topics

### Creating Log Stores

convenience init(url: URL) throws

Creates a log store based on a log archive.

class func local() throws -> Self

Creates a log store representing the Mac’s local store.

### Accessing Position

func position(date: Date) -> OSLogPosition

Returns a position representing the time specified.

func position(timeIntervalSinceEnd: TimeInterval) -> OSLogPosition

Returns a position representing time since the end of the time range that the entries span.

func position(timeIntervalSinceLatestBoot: TimeInterval) -> OSLogPosition

Returns a position representing time since the last boot in the series of entries.

### Accessing Entries

func getEntries(with: OSLogEnumerator.Options, at: OSLogPosition?, matching: NSPredicate?) throws -> AnySequence&lt;OSLogEntry>

Returns a sequence of log entries filtered by the parameters passed in.

### Initializers

init()Deprecated

convenience init(scope: OSLogStore.Scope) throws

### Enumerations

enum Scope

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

## See Also

### Read Log Entries

class OSLogEnumerator

An enumerator that can access and list log entries.

