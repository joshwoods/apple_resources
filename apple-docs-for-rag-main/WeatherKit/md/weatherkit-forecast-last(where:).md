

- WeatherKit
- Forecast
-  last(where:) 

Instance Method

# last(where:)

Returns the last element of the sequence that satisfies the given predicate.

WeatherKitSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func last(where predicate: (Self.Element) throws -> Bool) rethrows -> Self.Element?
```

## Parameters 

`predicate`  

A closure that takes an element of the sequence as its argument and returns a Boolean value indicating whether the element is a match.

## Return Value

The last element of the sequence that satisfies `predicate`, or `nil` if there is no element that satisfies `predicate`.

## Discussion

This example uses the `last(where:)` method to find the last negative number in an array of integers:

```
let numbers = [3, 7, 4, -2, 9, -6, 10, 1]
if let lastNegative = numbers.last(where: { $0 

Complexity

O(*n*), where *n* is the length of the collection.

