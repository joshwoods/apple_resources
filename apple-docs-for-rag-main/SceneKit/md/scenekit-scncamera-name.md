

- SceneKit
- SCNCamera
-  name 

Instance Property

# name

A name associated with the camera object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var name: String? { get set }
```

## Discussion

You can provide a descriptive name for a camera object to make managing your scene graph easier. Cameras loaded from a scene file may have names assigned by an artist using a 3D authoring tool. Use the SCNSceneSource class to examine cameras in a scene file without loading its scene graph.

Camera names are saved when you export a scene to a file using its write(to:options:delegate:progressHandler:) method. These names also appear in the Xcode scene editor. The SceneKit statistics view (see showsStatistics) shows the names of nodes with attached camera objects (which may not match the names of the attached camera objects themselves).

