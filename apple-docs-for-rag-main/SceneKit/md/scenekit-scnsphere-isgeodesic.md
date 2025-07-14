

- SceneKit
- SCNSphere
-  isGeodesic 

Instance Property

# isGeodesic

A Boolean value specifying whether SceneKit uses a geodesic polygon mesh to render the sphere.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var isGeodesic: Bool { get set }
```

## Discussion

The default value is false, specifying that SceneKit constructs a sphere mesh using a rectangular grid, like the lines of latitude and longitude on a globe of the Earth. This type of sphere mesh is efficient for most uses, but can cause texture distortion in the areas near its poles.

A value of true specifies that SceneKit constructs a sphere mesh by successively subdividing an icosahedron, creating a grid of uniformly sized triangles across the entire surface of the sphere, as shown below.

## See Also

### Adjusting Geometric Detail

var segmentCount: Int

A number determining the detail of the polygon mesh SceneKit uses to render the sphere. Animatable.

