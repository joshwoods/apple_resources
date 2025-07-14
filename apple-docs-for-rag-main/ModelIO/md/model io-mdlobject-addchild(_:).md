

- Model I/O
- MDLObject
-  addChild(\_:) 

Instance Method

# addChild(\_:)

Adds a child object to this object, creating a container for the object’s children if necessary.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func addChild(_ child: MDLObject)
```

## Parameters 

`child`  

The child object to add.

## Discussion

Many asset formats describe a hierarchy of transforms that model the spatial relationships between meshes, lights, and cameras in the asset. In such formats, hierarchic transforms are MDLObject instances whose children property references the objects affected by the transform—and those objects can be other MDLObject instances with children of their own.

If the object’s children property is `nil`, this method sets that property to a new MDLObjectContainer instance before adding the child object.

## See Also

### Working with Object Hierarchies

var parent: MDLObject?

The parent object that contains this object.

var children: any MDLObjectContainerComponent

A component that manages this object’s collection of children.

func enumerateChildObjects(of: AnyClass, root: MDLObject, using: (MDLObject, UnsafeMutablePointer&lt;ObjCBool>) -> Void, stopPointer: UnsafeMutablePointer&lt;ObjCBool>)

Executes the specified block using each object in this object’s child hierarchy.

var path: String

A path that identifies the object in an asset’s object hierarchy using object names.

func atPath(String) -> MDLObject

Returns the child object at the specified path.

