

- PHASE
- PHASEObject
-  addChild(\_:) 

Instance Method

# addChild(\_:)

Adds the given object as a child.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func addChild(_ child: PHASEObject) throws
```

## Parameters 

`child`  

The object to add to the children array.

## Mentioned in 

Playing sound from a location in a 3D scene

## Discussion

This function throws an error if `child` already has a different parent.

## See Also

### Managing the Hierarchy

var children: [PHASEObject]

Objects that position and orient in the scene relative to the given object.

var parent: PHASEObject?

The object that this instance positions and orients relative to in the scene.

func removeChild(PHASEObject)

Removes the given object as a child.

func removeChildren()

Removes all child objects from the given object.

