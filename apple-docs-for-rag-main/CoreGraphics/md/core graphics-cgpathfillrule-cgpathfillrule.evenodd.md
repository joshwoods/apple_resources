

- Core Graphics
- CGPathFillRule
-  CGPathFillRule.evenOdd 

Case

# CGPathFillRule.evenOdd

A rule that considers a region to be interior to a path based on the number of times it is enclosed by path elements.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case evenOdd
```

## Discussion

This rule plots a ray from any region to be evaluated toward the bounds of the drawing, then counts the closed path elements that the ray crosses. The rule defines interior regions as those where the sum of crossings is an odd number, and exterior regions as those where the sum of crossings is an even number.

## See Also

### Enumeration Cases

case winding

A rule that considers a region to be interior to a path if the winding number for that region is nonzero.

