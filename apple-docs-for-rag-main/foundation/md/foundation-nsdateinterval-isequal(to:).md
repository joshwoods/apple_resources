

- Foundation
- NSDateInterval
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Indicates whether the receiver is equal to the specified date interval.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func isEqual(to dateInterval: DateInterval) -> Bool
```

## Parameters 

`dateInterval`  

The date interval with which to check the receiver for equality.

## Return Value

true if the startDate and duration of `dateInterval` and the receiver are equal. Otherwise, false.

## See Also

### Comparing Date Intervals

func compare(DateInterval) -> ComparisonResult

Compares the receiver with the specified date interval.

