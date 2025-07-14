

- WeatherKit
- Forecast
-  ranges(of:) 

Instance Method

# ranges(of:)

Finds and returns the ranges of the all occurrences of a given sequence within the collection.

WeatherKitSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func ranges(of other: C) -> [Range] where C : Collection, Self.Element == C.Element
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`other`  

The sequence to search for.

## Return Value

A collection of ranges of all occurrences of `other`. Returns an empty collection if `other` is not found.

