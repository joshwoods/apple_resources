

- Objective-C Runtime
-  object_setClass(\_:\_:) 

Function

# object_setClass(\_:\_:)

Sets the class of an object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func object_setClass(
    _ obj: Any?,
    _ cls: AnyClass
) -> AnyClass?
```

## Parameters 

`obj`  

The object to modify.

`cls`  

A class object.

## Return Value

The previous value of `object`’s class, or `Nil` if `object` is `nil`.

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

func object_getClass(Any?) -> AnyClass?

Returns the class of an object.

