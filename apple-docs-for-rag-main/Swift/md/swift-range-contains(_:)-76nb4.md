

- Swift
- Range
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether the given element is contained within the range.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func contains(_ element: Bound) -> Bool
```

## Parameters 

`element`  

The element to check for containment.

## Return Value

`true` if `element` is contained in the range; otherwise, `false`.

## Discussion

Because `Range` represents a half-open range, a `Range` instance does not contain its upper bound. `element` is contained in the range if it is greater than or equal to the lower bound and less than the upper bound.

