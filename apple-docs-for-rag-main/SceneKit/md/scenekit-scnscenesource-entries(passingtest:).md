

- SceneKit
- SCNSceneSource
-  entries(passingTest:) 

Instance Method

# entries(passingTest:)

Loads and returns all objects in the scene source that pass the test in a given block.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
func entries(passingTest predicate: (Any, String, UnsafeMutablePointer) -> Bool) -> [Any]
```

## Parameters 

`predicate`  

The block to be applied to each object in the scene source.

The block takes three parameters:

entry  
The object to be tested.

identifier  
The unique identifier of the object in the scene source.

stop  
A reference to a Boolean value. Set `*stop` to true within the block to abort further processing of the scene source’s contents.

The block returns a Boolean value indicating whether the entry object passed the test and should be included in the method’s returned array.

## Return Value

An array of SceneKit objects from the scene source that pass the test.

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

Use this method to selectively load objects from a scene source matching criteria you specify. For example, the following code loads from a scene file only the nodes that have attached geometry:

```
NSArray *geometryNodes = [sceneSource entriesPassingTest:^BOOL(id entry, NSString *identifier, BOOL *stop) {
    if ([entry isKindOfClass:[SCNNode class]]) {
        SCNNode *node = (SCNNode *)entry;
        return (node.geometry != nil);
    } else {
        return NO;
    }
}];
```

## See Also

### Loading and Inspecting Scene Elements

func identifiersOfEntries(withClass: AnyClass) -> [String]

Returns the identifiers for all objects in the scene source of the specified class.

func entryWithIdentifier&lt;T>(String, withClass: T.Type) -> T?

Loads and returns a specific object in the scene source.

