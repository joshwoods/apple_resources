

- Objective-C Runtime
-  objc_removeAssociatedObjects(\_:) 

Function

# objc_removeAssociatedObjects(\_:)

Removes all associations for a given object.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_removeAssociatedObjects(_ object: Any)
```

## Parameters 

`object`  

An object that maintains associated objects.

## Discussion

The main purpose of this function is to make it easy to return an object to a “pristine state”. You should not use this function for general removal of associations from objects, since it also removes associations that other clients may have added to the object. Typically you should use objc_setAssociatedObject(_:_:_:_:) with a `nil` value to clear an association.

## See Also

### Associative References

func objc_setAssociatedObject(Any, UnsafeRawPointer, Any?, objc_AssociationPolicy)

Sets an associated value for a given object using a given key and association policy.

func objc_getAssociatedObject(Any, UnsafeRawPointer) -> Any?

Returns the value associated with a given object for a given key.

