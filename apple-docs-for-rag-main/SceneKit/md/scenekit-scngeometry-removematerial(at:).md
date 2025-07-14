

- SceneKit
- SCNGeometry
-  removeMaterial(at:) 

Instance Method

# removeMaterial(at:)

Removes a material attached to the geometry.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func removeMaterial(at index: Int)
```

## Parameters 

`index`  

The index of the attached material to be removed.

Important

Raises an exception (rangeException) if `index` is beyond the bounds of the materials array.

## See Also

### Managing a Geometry’s Materials

var materials: [SCNMaterial]

An array of SCNMaterial objects that determine the geometry’s appearance when rendered.

var firstMaterial: SCNMaterial?

The first material attached to the geometry.

func material(named: String) -> SCNMaterial?

Returns the first material attached to the geometry with the specified name.

func insertMaterial(SCNMaterial, at: Int)

Attaches a material to the geometry at the specified index.

func replaceMaterial(at: Int, with: SCNMaterial)

Replaces a material attached to the geometry with another.

