

- Objective-C Runtime
-  object_getClassName(\_:) 

Function

# object_getClassName(\_:)

Returns the class name of a given object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func object_getClassName(_ obj: Any?) -> UnsafePointer
```

## Parameters 

`obj`  

An Objective-C object.

## Return Value

The name of the class of which `obj` is an instance.

## See Also

### Working with Instances

func object_getIndexedIvars(Any?) -> UnsafeMutableRawPointer?

Returns a pointer to any extra bytes allocated with a instance given object.

func object_getIvar(Any?, Ivar) -> Any?

Reads the value of an instance variable in an object.

func object_setIvar(Any?, Ivar, Any?)

Sets the value of an instance variable in an object.

func object_getClass(Any?) -> AnyClass?

Returns the class of an object.

func object_setClass(Any?, AnyClass) -> AnyClass?

Sets the class of an object.

