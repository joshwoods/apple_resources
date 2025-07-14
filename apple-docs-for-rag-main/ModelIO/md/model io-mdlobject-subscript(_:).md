

- Model I/O
- MDLObject
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
subscript(key: Protocol) -> (any MDLComponent)? { get set }
```

## See Also

### Object Instancing

func atPath(String) -> MDLObject

Returns the child object at the specified path.

func enumerateChildObjects(of: AnyClass, root: MDLObject, using: (MDLObject, UnsafeMutablePointer&lt;ObjCBool>) -> Void, stopPointer: UnsafeMutablePointer&lt;ObjCBool>)

Executes the specified block using each object in this object’s child hierarchy.

