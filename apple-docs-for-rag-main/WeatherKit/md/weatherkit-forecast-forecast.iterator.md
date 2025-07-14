

- WeatherKit
- Forecast
-  Forecast.Iterator 

Type Alias

# Forecast.Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
typealias Iterator = IndexingIterator>
```

## Discussion

By default, a collection conforms to the `Sequence` protocol by supplying `IndexingIterator` as its associated `Iterator` type.

