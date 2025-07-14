

- PHASE
- PHASEEngine
-  unitsPerSecond 

Instance Property

# unitsPerSecond

A conversion factor from seconds to your app’s preferred unit of time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var unitsPerSecond: Double { get set }
```

## Discussion

Time-based properties throughout the framework apply the value you supply for this property to their value.

## See Also

### Measuring Units

var unitsPerMeter: Double

A conversion factor from meters to your app’s preferred unit of measurement.

