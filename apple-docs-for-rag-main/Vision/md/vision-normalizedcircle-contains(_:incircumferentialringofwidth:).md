

- Vision
- NormalizedCircle
-  contains(\_:inCircumferentialRingOfWidth:) 

Instance Method

# contains(\_:inCircumferentialRingOfWidth:)

Returns a Boolean value that indicates whether a ring around this circle’s circumference contains the specified point.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func contains(
    _ point: NormalizedPoint,
    inCircumferentialRingOfWidth ringWidth: CGFloat
) -> Bool
```

## Parameters 

`point`  

The normalized point.

`ringWidth`  

The ring width.

## See Also

### Determining whether the circle contains a point

func contains(NormalizedPoint) -> Bool

Returns a Boolean value that indicates whether this circle, including its boundary, contains the specified point.

