

- Model I/O
- MDLObject
-  children 

Instance Property

# children

A component that manages this object’s collection of children.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var children: any MDLObjectContainerComponent { get set }
```

## Discussion

Many asset formats describe a hierarchy of transforms that model the spatial relationships between meshes, lights, and cameras in the asset. In such formats, hierarchic transforms are MDLObject instances whose children property references the objects affected by the transform, and those objects can be other MDLObject instances with children of their own.

This property’s value is a component object—either a MDLObjectContainer instance, or a custom class that adopts the MDLObjectContainerComponent protocol. By default, an object has no container component (that is, this property’s value is `nil`). To add a container component, either write to this property an instance of a container component class or call the addChild(_:) method to create a default MDLObjectContainer instance and add a child object to that container.

Note

Reading or writing this property is equivalent to calling the componentConforming(to:) or setComponent(_:for:) method with the MDLObjectContainerComponent protocol.

Container components support fast enumeration and subscripting, so you can treat an object’s children property similarly to an array.

## See Also

### Working with Object Hierarchies

var parent: MDLObject?

The parent object that contains this object.

func addChild(MDLObject)

Adds a child object to this object, creating a container for the object’s children if necessary.

func enumerateChildObjects(of: AnyClass, root: MDLObject, using: (MDLObject, UnsafeMutablePointer&lt;ObjCBool>) -> Void, stopPointer: UnsafeMutablePointer&lt;ObjCBool>)

Executes the specified block using each object in this object’s child hierarchy.

var path: String

A path that identifies the object in an asset’s object hierarchy using object names.

func atPath(String) -> MDLObject

Returns the child object at the specified path.

