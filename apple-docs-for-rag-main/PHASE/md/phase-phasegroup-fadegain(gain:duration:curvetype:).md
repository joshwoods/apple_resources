

- PHASE
- PHASEGroup
-  fadeGain(gain:duration:curveType:) 

Instance Method

# fadeGain(gain:duration:curveType:)

Adjusts the volume of the sounds in a group gradually.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func fadeGain(
    gain: Double,
    duration: Double,
    curveType: PHASECurveType
)
```

## Parameters 

`gain`  

The target volume.

`duration`  

The total time to complete the volume adjustment. The framework scales this value by unitsPerSecond.

`curveType`  

A selection that specifies a mathematical curve that shapes the volume adjustment over time.

## See Also

### Conrolling Loudness

var gain: Double

Modifies the volume of the group’s sounds.

