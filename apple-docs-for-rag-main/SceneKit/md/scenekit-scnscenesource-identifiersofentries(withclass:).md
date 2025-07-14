

- SceneKit
- SCNSceneSource
-  identifiersOfEntries(withClass:) 

Instance Method

# identifiersOfEntries(withClass:)

Returns the identifiers for all objects in the scene source of the specified class.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func identifiersOfEntries(withClass entryClass: AnyClass) -> [String]
```

## Parameters 

`entryClass`  

The class of objects to find identifiers for.

## Return Value

An array of NSString objects, each the unique identifier of an object in the scene source.

## Discussion

SceneKit recognizes objects of the following classes in scene files:

- CAAnimation

- NSImage

- SCNCamera

- SCNGeometry

- SCNLight

- SCNMaterial

- SCNMorpher

- SCNNode

- SCNScene

- SCNSkinner

Each object in a scene file has an identifier that is unique for its class. These identifiers are determined by the software that created the scene file—for example, they may be descriptive names assigned by an artist using 3D authoring tools. For SceneKit classes with a name property (such as nodes and geometries), the name of an object loaded from a scene file is based on its identifier in the scene file.

Use this method to enumerate all objects in a scene file of a specified class without loading the objects and their content. For example, the following code finds the identifiers for all animations stored in a scene source:

```
NSArray *animations = [sceneSource identifiersOfEntriesWithClass:[CAAnimation class]];
```

## See Also

### Loading and Inspecting Scene Elements

func entryWithIdentifier&lt;T>(String, withClass: T.Type) -> T?

Loads and returns a specific object in the scene source.

func entries(passingTest: (Any, String, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> [Any]

Loads and returns all objects in the scene source that pass the test in a given block.

