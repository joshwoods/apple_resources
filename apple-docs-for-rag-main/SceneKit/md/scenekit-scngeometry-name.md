

- SceneKit
- SCNGeometry
-  name 

Instance Property

# name

A name associated with the geometry object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var name: String? { get set }
```

## Discussion

You can provide a descriptive name for a geometry object to make managing your scene graph easier. Geometries loaded from a scene file may have names assigned by an artist using a 3D authoring tool. Use the SCNSceneSource class to examine geometries in a scene file without loading its scene graph.

Geometry names are saved when you export a scene to a file using its write(to:options:delegate:progressHandler:) method. They also appear in the Xcode scene editor.

## See Also

### Managing Geometry Attributes

protocol SCNBoundingVolume

Methods common to the SCNNode and SCNGeometry classes for measuring location and size.

