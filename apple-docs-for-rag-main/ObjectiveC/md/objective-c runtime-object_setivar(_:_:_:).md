

- Objective-C Runtime
-  object_setIvar(\_:\_:\_:) 

Function

# object_setIvar(\_:\_:\_:)

Sets the value of an instance variable in an object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func object_setIvar(
    _ obj: Any?,
    _ ivar: Ivar,
    _ value: Any?
)
```

## Parameters 

`obj`  

The object containing the instance variable whose value you want to set.

`ivar`  

The Ivar describing the instance variable whose value you want to set.

`value`  

The new value for the instance variable.

## Discussion

object_setIvar(_:_:_:) is faster than object_setInstanceVariable if the Ivar for the instance variable is already known.

## See Also

### Working with Instances

func object_getIndexedIvars(Any?) -> UnsafeMutableRawPointer?

Returns a pointer to any extra bytes allocated with a instance given object.

func object_getIvar(Any?, Ivar) -> Any?

Reads the value of an instance variable in an object.

func object_getClassName(Any?) -> UnsafePointer&lt;CChar>

Returns the class name of a given object.

func object_getClass(Any?) -> AnyClass?

Returns the class of an object.

func object_setClass(Any?, AnyClass) -> AnyClass?

Sets the class of an object.

