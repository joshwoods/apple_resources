

- Objective-C Runtime
-  objc_getAssociatedObject(\_:\_:) 

Function

# objc_getAssociatedObject(\_:\_:)

Returns the value associated with a given object for a given key.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_getAssociatedObject(
    _ object: Any,
    _ key: UnsafeRawPointer
) -> Any?
```

## Parameters 

`object`  

The source object for the association.

`key`  

The key for the association.

## Return Value

The value associated with the key `key` for `object`.

## See Also

### Associative References

func objc_setAssociatedObject(Any, UnsafeRawPointer, Any?, objc_AssociationPolicy)

Sets an associated value for a given object using a given key and association policy.

func objc_removeAssociatedObjects(Any)

Removes all associations for a given object.

