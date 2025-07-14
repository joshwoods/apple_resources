

- SceneKit
- SCNGeometry
-  material(named:) 

Instance Method

# material(named:)

Returns the first material attached to the geometry with the specified name.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func material(named name: String) -> SCNMaterial?
```

## Parameters 

`name`  

The name of the material to be retrieved.

## Return Value

A material object with the specified name.

## Discussion

You can use the name property of each SCNMaterial object to make managing your scene graph easier. Materials loaded from a scene file may have names assigned by an artist using a 3D authoring tool.

If a geometry has multiple materials attached with the same name, this method returns the first according to the order of the materials array.

## See Also

### Managing a Geometry’s Materials

var materials: [SCNMaterial]

An array of SCNMaterial objects that determine the geometry’s appearance when rendered.

var firstMaterial: SCNMaterial?

The first material attached to the geometry.

func insertMaterial(SCNMaterial, at: Int)

Attaches a material to the geometry at the specified index.

func removeMaterial(at: Int)

Removes a material attached to the geometry.

func replaceMaterial(at: Int, with: SCNMaterial)

Replaces a material attached to the geometry with another.

