

- SceneKit
- SCNGeometry
-  levelsOfDetail 

Instance Property

# levelsOfDetail

An array of SCNLevelOfDetail objects for managing the geometry’s appearance when viewed from far away.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var levelsOfDetail: [SCNLevelOfDetail]? { get set }
```

## Discussion

Because rendering a complex geometry incurs a performance cost, you can use level-of-detail objects to substitute simpler geometries in its place as its distance from the point of view camera increases (or its apparent size decreases). For details, see SCNLevelOfDetail.

## See Also

### Optimizing Level of Detail

class SCNLevelOfDetail

An alternate resolution for a geometry that SceneKit automatically substitutes to improve rendering performance.

