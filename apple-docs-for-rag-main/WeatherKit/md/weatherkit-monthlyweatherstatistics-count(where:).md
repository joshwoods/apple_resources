

- WeatherKit
- MonthlyWeatherStatistics
-  count(where:) 

Instance Method

# count(where:)

Returns the number of elements in the sequence that satisfy the given predicate.

WeatherKitSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func count(where predicate: (Self.Element) throws(E) -> Bool) throws(E) -> Int where E : Error
```

## Parameters 

`predicate`  

A closure that takes each element of the sequence as its argument and returns a Boolean value indicating whether the element should be included in the count.

## Return Value

The number of elements in the sequence that satisfy the given predicate.

## Discussion

You can use this method to count the number of elements that pass a test. The following example finds the number of names that are fewer than five characters long:

```
let names = ["Jacqueline", "Ian", "Amy", "Juan", "Soroush", "Tiffany"]
let shortNameCount = names.count(where: { $0.count 

To find the number of times a specific element appears in the sequence, use the equal to operator (`==`) in the closure to test for a match.

```
let birds = ["duck", "duck", "duck", "duck", "goose"]
let duckCount = birds.count(where: { $0 == "duck" })
// duckCount == 4
```

The sequence must be finite.

