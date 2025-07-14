

- Foundation
- Calendar
- Calendar.MatchingPolicy
-  Calendar.MatchingPolicy.strict 

Case

# Calendar.MatchingPolicy.strict

If specified, the algorithm travels as far forward or backward as necessary looking for a match.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case strict
```

## Discussion

For example, if searching for Feb 29 in the Gregorian calendar, the algorithm may choose March 1 instead (for example, if the year is not a leap year). If you wish to find the next Feb 29 without the algorithm adjusting the next higher component in the specified `DateComponents`, then use the `strict` option.

Note

There are ultimately implementation-defined limits in how far distant the search will go.

## See Also

### Enumeration Cases

case nextTime

If there is no matching time before the end of the next instance of the next higher component to the highest specified component in the `DateComponents` argument, the algorithm will return the next existing time which exists.

case nextTimePreservingSmallerComponents

If specified, and there is no matching time before the end of the next instance of the next higher component to the highest specified component in the `DateComponents` argument, the method returns the next existing value of the missing component and preserves the lower components’ values (for example, no 2:37am results in 3:37am, if that exists).

case previousTimePreservingSmallerComponents

If there is no matching time before the end of the next instance of the next higher component to the highest specified component in the `DateComponents` argument, the algorithm will return the previous existing value of the missing component and preserves the lower components’ values.

