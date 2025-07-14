

- SceneKit
- SCNSceneSource
-  entryWithIdentifier(\_:withClass:) 

Instance Method

# entryWithIdentifier(\_:withClass:)

Loads and returns a specific object in the scene source.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.8+tvOSvisionOSwatchOS

``` source
func entryWithIdentifier(
    _ uid: String,
    withClass entryClass: T.Type
) -> T? where T : AnyObject
```

## Parameters 

`uid`  

The unique identifier of an object in the scene source.

`entryClass`  

The class of object to load.

## Return Value

A new SceneKit object (of the specified class) containing the requested scene source entry, or `nil` if no such object exists in the scene source.

## Discussion

SceneKit recognizes objects of the following classes in scene files:

- CAAnimation

- NSImage (macOS) or UIImage (iOS/watchOS/tvOS)

- SCNCamera

- SCNGeometry

- SCNLight

- SCNMaterial

- SCNMorpher

- SCNNode

- SCNScene

- SCNSkinner

Each object in a scene file has an identifier that is unique for its class. These identifiers are determined by the software that created the scene file—for example, they may be descriptive names assigned by an artist using 3D authoring tools. For SceneKit classes with a `name` property (such as nodes and geometries), the name of an object loaded from a scene file is based on its identifier in the scene file.

If you don’t have the identifier for an object you want to load, use the identifiersOfEntries(withClass:) method to find the identifiers for objects in a scene file. You can also see the identifier for each object in a scene file when viewing it in Xcode’s scene editor.

Calling this method instantiates an object of the specified SceneKit class and loads all content from the scene file corresponding to the requested entry. Keep in mind that loading one SceneKit object may also load other objects and their contents, such as the lights, cameras, or geometries attached to a node.

For example, the following method finds the identifier for a geometry and then loads it (and any animations or materials attached to it):

```
func loadSpaceship(from sceneSource: SCNSceneSource) -> SCNGeometry? {
    let identifiers = sceneSource.identifiersOfEntries(withClass: SCNGeometry.self)
    guard let identifier = identifiers.filter({ $0.contains("spaceship") }).first
        else { return nil } // no matching identifier
    return sceneSource.entryWithIdentifier(identifier, withClass: SCNGeometry.self)
}
```

## See Also

### Loading and Inspecting Scene Elements

func identifiersOfEntries(withClass: AnyClass) -> [String]

Returns the identifiers for all objects in the scene source of the specified class.

func entries(passingTest: (Any, String, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> [Any]

Loads and returns all objects in the scene source that pass the test in a given block.

