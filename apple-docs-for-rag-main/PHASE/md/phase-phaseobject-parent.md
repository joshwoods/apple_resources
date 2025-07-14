

- PHASE
- PHASEObject
-  parent 

Instance Property

# parent

The object that this instance positions and orients relative to in the scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
weak var parent: PHASEObject? { get }
```

## See Also

### Managing the Hierarchy

var children: [PHASEObject]

Objects that position and orient in the scene relative to the given object.

func addChild(PHASEObject) throws

Adds the given object as a child.

func removeChild(PHASEObject)

Removes the given object as a child.

func removeChildren()

Removes all child objects from the given object.

