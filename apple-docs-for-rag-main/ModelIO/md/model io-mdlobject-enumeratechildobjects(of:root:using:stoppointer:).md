

- Model I/O
- MDLObject
-  enumerateChildObjects(of:root:using:stopPointer:) 

Instance Method

# enumerateChildObjects(of:root:using:stopPointer:)

Executes the specified block using each object in this object’s child hierarchy.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func enumerateChildObjects(
    of objectClass: AnyClass,
    root: MDLObject,
    using block: @escaping (MDLObject, UnsafeMutablePointer) -> Void,
    stopPointer: UnsafeMutablePointer
)
```

## Parameters 

`objectClass`  

A Model I/O class representing a type of child objects to evaluate. For example, pass the MDLMesh class to evaluate all 3D objects stored in the asset. Pass the MDLObject class to evaluate all child objects regardless of type.

`root`  

The root object at which to begin traversing the child object hierarchy.

`block`  

The block to apply to child objects. This block takes two parameters: the `object` to be evaluated by the block, and a `stop` pointer that you can set to true to stop further evaluation of the object hierarchy.

`stopPointer`  

Set this pointer’s value to true during enumeration to stop further enumeration of the object hierarchy.

## See Also

### Working with Object Hierarchies

var parent: MDLObject?

The parent object that contains this object.

var children: any MDLObjectContainerComponent

A component that manages this object’s collection of children.

func addChild(MDLObject)

Adds a child object to this object, creating a container for the object’s children if necessary.

var path: String

A path that identifies the object in an asset’s object hierarchy using object names.

func atPath(String) -> MDLObject

Returns the child object at the specified path.

