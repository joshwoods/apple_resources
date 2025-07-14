

- SceneKit
- SCNGeometry
-  materials 

Instance Property

# materials

An array of SCNMaterial objects that determine the geometry’s appearance when rendered.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var materials: [SCNMaterial] { get set }
```

## Discussion

Materials provide the information SceneKit uses to add color, lighting, texture, and special effects when rendering a geometry. Each SCNMaterial object can be shared between several geometries.

If a geometry contains multiple elements (see elementCount), you can associate a separate material with each geometry element. For example, the teapot in Figure 1 has four elements, each with a different material.

If a geometry has the same number of materials as it has geometry elements, the material index corresponds to the element index. For geometries with fewer materials than elements, SceneKit determines the material index for each element by calculating the index of that element modulo the number of materials. For example, in a geometry with six elements and three materials, SceneKit renders the element at index `5` using the material at index `5 % 3 = 2`.

## See Also

### Managing a Geometry’s Materials

var firstMaterial: SCNMaterial?

The first material attached to the geometry.

func material(named: String) -> SCNMaterial?

Returns the first material attached to the geometry with the specified name.

func insertMaterial(SCNMaterial, at: Int)

Attaches a material to the geometry at the specified index.

func removeMaterial(at: Int)

Removes a material attached to the geometry.

func replaceMaterial(at: Int, with: SCNMaterial)

Replaces a material attached to the geometry with another.

