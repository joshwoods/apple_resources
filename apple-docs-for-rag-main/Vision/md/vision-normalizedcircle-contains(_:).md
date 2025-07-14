

- Vision
- NormalizedCircle
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether this circle, including its boundary, contains the specified point.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func contains(_ point: NormalizedPoint) -> Bool
```

## Parameters 

`point`  

The normalized point.

## See Also

### Determining whether the circle contains a point

func contains(NormalizedPoint, inCircumferentialRingOfWidth: CGFloat) -> Bool

Returns a Boolean value that indicates whether a ring around this circle’s circumference contains the specified point.

