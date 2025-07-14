

- PHASE
- PHASEGroup
-  fadeRate(rate:duration:curveType:) 

Instance Method

# fadeRate(rate:duration:curveType:)

Adjusts the playback speed of the sounds in a group gradually.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func fadeRate(
    rate: Double,
    duration: Double,
    curveType: PHASECurveType
)
```

## Parameters 

`rate`  

The target playback speed.

`duration`  

The total time to adjust the playback speed. The framework scales this value by unitsPerSecond.

`curveType`  

A selection that specifies a mathematical curve that shapes the playback speed adjustment over time.

## See Also

### Adjusting Playback Speed

var rate: Double

The group’s playback speed.

