

- Foundation
- Calendar
-  dates(byMatching:startingAt:in:matchingPolicy:repeatedTimePolicy:direction:) 

Instance Method

# dates(byMatching:startingAt:in:matchingPolicy:repeatedTimePolicy:direction:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
func dates(
    byMatching components: DateComponents,
    startingAt start: Date,
    in range: Range? = nil,
    matchingPolicy: Calendar.MatchingPolicy = .nextTime,
    repeatedTimePolicy: Calendar.RepeatedTimePolicy = .first,
    direction: Calendar.SearchDirection = .forward
) -> some Sendable & Sequence
```

