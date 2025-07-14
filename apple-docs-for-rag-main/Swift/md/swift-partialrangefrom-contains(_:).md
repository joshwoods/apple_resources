

- Swift
- PartialRangeFrom
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether the given element is contained within the range expression.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func contains(_ element: Bound) -> Bool
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`element`  

The element to check for containment.

## Return Value

`true` if `element` is contained in the range expression; otherwise, `false`.

