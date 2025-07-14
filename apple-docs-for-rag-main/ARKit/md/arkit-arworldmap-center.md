

- ARKit
- ARWorldMap
-  center 

Instance Property

# center

The center point of the world map’s space-mapping data, relative to the world coordinate origin of the session the map was recorded in.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var center: simd_float3 { get }
```

## Discussion

The extent and center properties together define a bounding box for the data recorded in the world map.

## See Also

### Examining a World Map

var anchors: [ARAnchor]

The set of anchors recorded in the world map.

var extent: simd_float3

The size of the world map’s space-mapping data, relative to the world coordinate origin of the session the map was recorded in.

