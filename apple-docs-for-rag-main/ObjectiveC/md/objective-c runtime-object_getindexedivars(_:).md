

- Objective-C Runtime
-  object_getIndexedIvars(\_:) 

Function

# object_getIndexedIvars(\_:)

Returns a pointer to any extra bytes allocated with a instance given object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func object_getIndexedIvars(_ obj: Any?) -> UnsafeMutableRawPointer?
```

## Parameters 

`obj`  

An Objective-C object.

## Return Value

A pointer to any extra bytes allocated with `obj`. If `obj` was not allocated with any extra bytes, then dereferencing the returned pointer is undefined.

## Discussion

This function returns a pointer to any extra bytes allocated with the instance (as specified by class_createInstance(_:_:) with extraBytes\>0). This memory follows the object’s ordinary ivars, but may not be adjacent to the last ivar.

The returned pointer is guaranteed to be pointer-size aligned, even if the area following the object’s last ivar is less aligned than that. Alignment greater than pointer-size is never guaranteed, even if the area following the object’s last ivar is more aligned than that.

In a garbage-collected environment, the memory is scanned conservatively.

## See Also

### Working with Instances

func object_getIvar(Any?, Ivar) -> Any?

Reads the value of an instance variable in an object.

func object_setIvar(Any?, Ivar, Any?)

Sets the value of an instance variable in an object.

func object_getClassName(Any?) -> UnsafePointer&lt;CChar>

Returns the class name of a given object.

func object_getClass(Any?) -> AnyClass?

Returns the class of an object.

func object_setClass(Any?, AnyClass) -> AnyClass?

Sets the class of an object.

