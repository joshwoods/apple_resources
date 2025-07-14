

- SceneKit
- SCNGeometry
-  insertMaterial(\_:at:) 

Instance Method

# insertMaterial(\_:at:)

Attaches a material to the geometry at the specified index.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func insertMaterial(
    _ material: SCNMaterial,
    at index: Int
)
```

## Parameters 

`material`  

The material to attach.

`index`  

The location in the geometry’s materials array at which to add the new material.

Important

Raises an exception (rangeException) if `index` is greater than the number of elements in the materials array.

## See Also

### Managing a Geometry’s Materials

var materials: [SCNMaterial]

An array of SCNMaterial objects that determine the geometry’s appearance when rendered.

var firstMaterial: SCNMaterial?

The first material attached to the geometry.

func material(named: String) -> SCNMaterial?

Returns the first material attached to the geometry with the specified name.

func removeMaterial(at: Int)

Removes a material attached to the geometry.

func replaceMaterial(at: Int, with: SCNMaterial)

Replaces a material attached to the geometry with another.

