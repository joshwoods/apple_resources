

- Objective-C Runtime
-  object_getClass(\_:) 

Function

# object_getClass(\_:)

Returns the class of an object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func object_getClass(_ obj: Any?) -> AnyClass?
```

## Parameters 

`obj`  

The object you want to inspect.

## Return Value

The class object of which `object` is an instance, or `Nil` if `object` is `nil`.

## See Also

### Working with Instances

func object_getIndexedIvars(Any?) -> UnsafeMutableRawPointer?

Returns a pointer to any extra bytes allocated with a instance given object.

func object_getIvar(Any?, Ivar) -> Any?

Reads the value of an instance variable in an object.

func object_setIvar(Any?, Ivar, Any?)

Sets the value of an instance variable in an object.

func object_getClassName(Any?) -> UnsafePointer&lt;CChar>

Returns the class name of a given object.

func object_setClass(Any?, AnyClass) -> AnyClass?

Sets the class of an object.

