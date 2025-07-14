

- SceneKit
- SCNLevelOfDetail
-  init(geometry:worldSpaceDistance:) 

Initializer

# init(geometry:worldSpaceDistance:)

Creates a level of detail with the specified geometry and threshold camera distance.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
convenience init(
    geometry: SCNGeometry?,
    worldSpaceDistance distance: CGFloat
)
```

## Parameters 

`geometry`  

The geometry to render for this level of detail, or `nil` if SceneKit should render no geometry at this level of detail.

`distance`  

The minimum distance from the current point of view for this level of detail to appear.

## Return Value

A level-of-detail object. You associate levels of detail with a SCNGeometry object using its levelsOfDetail property.

## Discussion

When rendering a geometry with associated levels of detail, SceneKit calculates the distance from the current point of view to the geometry’s parent node, then renders the geometry for the SCNLevelOfDetail object with the smallest `distance` parameter greater than that distance.

If you pass `nil` for the geometry parameter, SceneKit renders no geometry for the level of detail. Creating a level-of-detail object with no geometry allows you to skip rendering costs entirely for an object when it would appear very far away or very small.

## See Also

### Creating a Level of Detail

convenience init(geometry: SCNGeometry?, screenSpaceRadius: CGFloat)

Creates a level of detail with the specified geometry and threshold pixel radius.

