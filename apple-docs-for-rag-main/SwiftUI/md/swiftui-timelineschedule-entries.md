

- SwiftUI
- TimelineSchedule
-  Entries 

Associated Type

# Entries

The sequence of dates within a schedule.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
associatedtype Entries : Sequence where Self.Entries.Element == Date
```

**Required**

## Discussion

The entries(from:mode:) method returns a value of this type, which is a Sequence of dates in ascending order. A TimelineView that you create with a schedule updates its content at the moments in time corresponding to the dates included in the sequence.

## See Also

### Getting a sequence of dates

func entries(from: Date, mode: Self.Mode) -> Self.Entries

Provides a sequence of dates starting around a given date.

**Required**

