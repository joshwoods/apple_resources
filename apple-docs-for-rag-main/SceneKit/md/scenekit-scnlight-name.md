

- SceneKit
- SCNLight
-  name 

Instance Property

# name

A name associated with the light.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var name: String? { get set }
```

## Discussion

You can provide a descriptive name for a light to make managing your scene graph easier. Lights loaded from a scene file may have names assigned by an artist using a 3D authoring tool. To examine lights in a scene file without loading its scene graph, use the SCNSceneSource class.

Light names are saved when you export a scene to a file using its write(to:options:delegate:progressHandler:) method. Light names also appear in the Xcode scene editor.

## See Also

### Managing Light Attributes

func attribute(forKey: String) -> Any?

Returns the value of a lighting attribute.

Deprecated

func setAttribute(Any?, forKey: String)

Sets the value for a lighting attribute.

Deprecated

Lighting Attribute Keys

Keys for specifying the behavior of a light using the attribute(forKey:) and setAttribute(_:forKey:) methods.

