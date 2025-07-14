

- Objective-C Runtime
-  object_getIvar(\_:\_:) 

Function

# object_getIvar(\_:\_:)

Reads the value of an instance variable in an object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func object_getIvar(
    _ obj: Any?,
    _ ivar: Ivar
) -> Any?
```

## Parameters 

`obj`  

The object containing the instance variable whose value you want to read.

`ivar`  

The Ivar describing the instance variable whose value you want to read.

## Return Value

The value of the instance variable specified by `ivar`, or `nil` if `object` is `nil`.

## Discussion

object_getIvar(_:_:) is faster than object_getInstanceVariable if the Ivar for the instance variable is already known.

## See Also

### Working with Instances

func object_getIndexedIvars(Any?) -> UnsafeMutableRawPointer?

Returns a pointer to any extra bytes allocated with a instance given object.

func object_setIvar(Any?, Ivar, Any?)

Sets the value of an instance variable in an object.

func object_getClassName(Any?) -> UnsafePointer&lt;CChar>

Returns the class name of a given object.

func object_getClass(Any?) -> AnyClass?

Returns the class of an object.

func object_setClass(Any?, AnyClass) -> AnyClass?

Sets the class of an object.

