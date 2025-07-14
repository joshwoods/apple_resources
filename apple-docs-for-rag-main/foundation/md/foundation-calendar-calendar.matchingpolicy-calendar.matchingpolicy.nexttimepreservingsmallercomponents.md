

- Foundation
- Calendar
- Calendar.MatchingPolicy
-  Calendar.MatchingPolicy.nextTimePreservingSmallerComponents 

Case

# Calendar.MatchingPolicy.nextTimePreservingSmallerComponents

If specified, and there is no matching time before the end of the next instance of the next higher component to the highest specified component in the `DateComponents` argument, the method returns the next existing value of the missing component and preserves the lower components’ values (for example, no 2:37am results in 3:37am, if that exists).

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case nextTimePreservingSmallerComponents
```

## See Also

### Enumeration Cases

case nextTime

If there is no matching time before the end of the next instance of the next higher component to the highest specified component in the `DateComponents` argument, the algorithm will return the next existing time which exists.

case previousTimePreservingSmallerComponents

If there is no matching time before the end of the next instance of the next higher component to the highest specified component in the `DateComponents` argument, the algorithm will return the previous existing value of the missing component and preserves the lower components’ values.

case strict

If specified, the algorithm travels as far forward or backward as necessary looking for a match.

