

- SceneKit
- SCNGeometry
-  replaceMaterial(at:with:) 

Instance Method

# replaceMaterial(at:with:)

Replaces a material attached to the geometry with another.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func replaceMaterial(
    at index: Int,
    with material: SCNMaterial
)
```

## Parameters 

`index`  

The index of the attached material to be replaced.

Important

Raises an exception (rangeException) if `index` is beyond the bounds of the materials array.

`material`  

The material with which to replace the attached material.

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

func removeMaterial(at: Int)

Removes a material attached to the geometry.

