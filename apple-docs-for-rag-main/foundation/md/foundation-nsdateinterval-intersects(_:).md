

- Foundation
- NSDateInterval
-  intersects(\_:) 

Instance Method

# intersects(\_:)

Indicates whether the receiver intersects with the specified date interval.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func intersects(_ dateInterval: DateInterval) -> Bool
```

## Parameters 

`dateInterval`  

The date interval with which to check the receiver for intersection.

## Discussion

See intersection(with:) for more information about determining whether two date intervals intersect.

## See Also

### Determining Intersections

func intersection(with: DateInterval) -> DateInterval?

Returns the intersection between the receiver and the specified date interval.

