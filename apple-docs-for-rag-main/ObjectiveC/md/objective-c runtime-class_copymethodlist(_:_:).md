

- Objective-C Runtime
-  class_copyMethodList(\_:\_:) 

Function

# class_copyMethodList(\_:\_:)

Describes the instance methods implemented by a class.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func class_copyMethodList(
    _ cls: AnyClass?,
    _ outCount: UnsafeMutablePointer?
) -> UnsafeMutablePointer?
```

## Parameters 

`cls`  

The class you want to inspect.

`outCount`  

On return, contains the length of the returned array. If `outCount` is `NULL`, the length is not returned.

## Return Value

An array of pointers of type `Method` describing the instance methods implemented by the class—any instance methods implemented by superclasses are not included. The array contains `*outCount` pointers followed by a `NULL` terminator. You must free the array with `free()`.

If `cls` implements no instance methods, or `cls` is `Nil`, returns `NULL` and `*outCount` is `0`.

## Discussion

To get the class methods of a class, use `class_copyMethodList(object_getClass(cls), &count)`.

To get the implementations of methods that may be implemented by superclasses, use class_getInstanceMethod(_:_:) or class_getClassMethod(_:_:).

## See Also

### Working with Classes

func class_getName(AnyClass?) -> UnsafePointer&lt;CChar>

Returns the name of a class.

func class_getSuperclass(AnyClass?) -> AnyClass?

Returns the superclass of a class.

func class_setSuperclass(AnyClass, AnyClass) -> AnyClass

Sets the superclass of a given class.

Deprecated

func class_isMetaClass(AnyClass?) -> Bool

Returns a Boolean value that indicates whether a class object is a metaclass.

func class_getInstanceSize(AnyClass?) -> Int

Returns the size of instances of a class.

func class_getInstanceVariable(AnyClass?, UnsafePointer&lt;CChar>) -> Ivar?

Returns the `Ivar` for a specified instance variable of a given class.

func class_getClassVariable(AnyClass?, UnsafePointer&lt;CChar>) -> Ivar?

Returns the `Ivar` for a specified class variable of a given class.

func class_addIvar(AnyClass?, UnsafePointer&lt;CChar>, Int, UInt8, UnsafePointer&lt;CChar>?) -> Bool

Adds a new instance variable to a class.

func class_copyIvarList(AnyClass?, UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;Ivar>?

Describes the instance variables declared by a class.

func class_getIvarLayout(AnyClass?) -> UnsafePointer&lt;UInt8>?

Returns a description of the `Ivar` layout for a given class.

func class_setIvarLayout(AnyClass?, UnsafePointer&lt;UInt8>?)

Sets the `Ivar` layout for a given class.

func class_getWeakIvarLayout(AnyClass?) -> UnsafePointer&lt;UInt8>?

Returns a description of the layout of weak `Ivar`s for a given class.

func class_setWeakIvarLayout(AnyClass?, UnsafePointer&lt;UInt8>?)

Sets the layout for weak `Ivar`s for a given class.

func class_getProperty(AnyClass?, UnsafePointer&lt;CChar>) -> objc_property_t?

Returns a property with a given name of a given class.

func class_copyPropertyList(AnyClass?, UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;objc_property_t>?

Describes the properties declared by a class.

