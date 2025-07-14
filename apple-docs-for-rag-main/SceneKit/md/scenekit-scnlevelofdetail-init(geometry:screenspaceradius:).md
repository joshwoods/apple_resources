

- SceneKit
- SCNLevelOfDetail
-  init(geometry:screenSpaceRadius:) 

Initializer

# init(geometry:screenSpaceRadius:)

Creates a level of detail with the specified geometry and threshold pixel radius.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
convenience init(
    geometry: SCNGeometry?,
    screenSpaceRadius radius: CGFloat
)
```

## Parameters 

`geometry`  

The geometry to render for this level of detail.

`radius`  

The maximum radius (in pixels) of the geometry’s bounding sphere for this level of detail to appear.

## Return Value

A level-of-detail object. You associate levels of detail with a SCNGeometry object using its levelsOfDetail property.

## Discussion

When rendering a geometry with associated levels of detail, SceneKit calculates the radius in pixels of the circle covered by a geometry’s bounding sphere, then renders the geometry for the SCNLevelOfDetail object with the largest `radius` parameter smaller than that circle.

If you pass `nil` for the geometry parameter, SceneKit renders no geometry for the level of detail. Creating a level-of-detail object with no geometry allows you to skip rendering costs entirely for an object when it would appear very far away or very small.

## See Also

### Creating a Level of Detail

convenience init(geometry: SCNGeometry?, worldSpaceDistance: CGFloat)

Creates a level of detail with the specified geometry and threshold camera distance.

