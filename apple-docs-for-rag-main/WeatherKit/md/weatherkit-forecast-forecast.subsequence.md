

- WeatherKit
- Forecast
-  Forecast.SubSequence 

Type Alias

# Forecast.SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
typealias SubSequence = Slice>
```

## Discussion

The default subsequence type for collections that don’t define their own is `Slice`.

