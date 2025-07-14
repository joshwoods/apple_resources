

- Model I/O
- MDLObject
-  atPath(\_:) 

Instance Method

# atPath(\_:)

Returns the child object at the specified path.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func atPath(_ path: String) -> MDLObject
```

## Parameters 

`path`  

A path that identifies the object to be found using object names.

## Return Value

The requested object, or `nil` if no object matching the path can be found.

## Discussion

See the path property for examples of how to construct object paths for searching.

## See Also

### Working with Object Hierarchies

var parent: MDLObject?

The parent object that contains this object.

var children: any MDLObjectContainerComponent

A component that manages this object’s collection of children.

func addChild(MDLObject)

Adds a child object to this object, creating a container for the object’s children if necessary.

func enumerateChildObjects(of: AnyClass, root: MDLObject, using: (MDLObject, UnsafeMutablePointer&lt;ObjCBool>) -> Void, stopPointer: UnsafeMutablePointer&lt;ObjCBool>)

Executes the specified block using each object in this object’s child hierarchy.

var path: String

A path that identifies the object in an asset’s object hierarchy using object names.

