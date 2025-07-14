

- SceneKit
- SCNMaterial
-  name 

Instance Property

# name

A name associated with the material.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var name: String? { get set }
```

## Discussion

You can provide a descriptive name for a material to make managing your scene graph easier. Materials loaded from a scene file may have names assigned by an artist using a 3D authoring tool. Use the SCNSceneSource class to examine materials in a scene file without loading its scene graph.

Material names are saved when you export a scene to a file using its write(to:options:delegate:progressHandler:) method, and appear in the Xcode scene editor.

