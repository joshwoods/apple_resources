

- SceneKit
- SCNGeometry
-  firstMaterial 

Instance Property

# firstMaterial

The first material attached to the geometry.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var firstMaterial: SCNMaterial? { get set }
```

## Discussion

Calling this convenience method is equivalent to retrieving the first object from the geometry’s materials array. This property’s value is `nil` if the geometry has no attached materials.

## See Also

### Managing a Geometry’s Materials

var materials: [SCNMaterial]

An array of SCNMaterial objects that determine the geometry’s appearance when rendered.

func material(named: String) -> SCNMaterial?

Returns the first material attached to the geometry with the specified name.

func insertMaterial(SCNMaterial, at: Int)

Attaches a material to the geometry at the specified index.

func removeMaterial(at: Int)

Removes a material attached to the geometry.

func replaceMaterial(at: Int, with: SCNMaterial)

Replaces a material attached to the geometry with another.

