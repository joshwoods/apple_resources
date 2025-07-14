

- Objective-C Runtime
-  objc_setAssociatedObject(\_:\_:\_:\_:) 

Function

# objc_setAssociatedObject(\_:\_:\_:\_:)

Sets an associated value for a given object using a given key and association policy.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_setAssociatedObject(
    _ object: Any,
    _ key: UnsafeRawPointer,
    _ value: Any?,
    _ policy: objc_AssociationPolicy
)
```

## Parameters 

`object`  

The source object for the association.

`key`  

The key for the association.

`value`  

The value to associate with the key `key` for `object`. Pass `nil` to clear an existing association.

`policy`  

The policy for the association. For possible values, see objc_AssociationPolicy.

## See Also

### Associative References

func objc_getAssociatedObject(Any, UnsafeRawPointer) -> Any?

Returns the value associated with a given object for a given key.

func objc_removeAssociatedObjects(Any)

Removes all associations for a given object.

