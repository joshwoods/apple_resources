

- PHASE
- PHASEObject
-  children 

Instance Property

# children

Objects that position and orient in the scene relative to the given object.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var children: [PHASEObject] { get }
```

## Discussion

To manage members of this array, use addChild(_:), removeChild(_:), and removeChildren().

## See Also

### Managing the Hierarchy

var parent: PHASEObject?

The object that this instance positions and orients relative to in the scene.

func addChild(PHASEObject) throws

Adds the given object as a child.

func removeChild(PHASEObject)

Removes the given object as a child.

func removeChildren()

Removes all child objects from the given object.

