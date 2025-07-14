

- Objective-C Runtime
-  class_replaceMethod(\_:\_:\_:\_:) 

Function

# class_replaceMethod(\_:\_:\_:\_:)

Replaces the implementation of a method for a given class.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func class_replaceMethod(
    _ cls: AnyClass?,
    _ name: Selector,
    _ imp: IMP,
    _ types: UnsafePointer?
) -> IMP?
```

## Parameters 

`cls`  

The class you want to modify.

`name`  

A selector that identifies the method whose implementation you want to replace.

`imp`  

The new implementation for the method identified by `name` for the class identified by `cls`.

`types`  

An array of characters that describe the types of the arguments to the method. For possible values, see Objective-C Runtime Programming Guide \> Type Encodings. Since the function must take at least two arguments—`self` and `_cmd`, the second and third characters must be “`@:`” (the first character is the return type).

## Return Value

The previous implementation of the method identified by `name` for the class identified by `cls`.

## Discussion

This function behaves in two different ways:

- If the method identified by `name` does not yet exist, it is added as if class_addMethod(_:_:_:_:) were called. The type encoding specified by `types` is used as given.

- If the method identified by `name` does exist, its IMP is replaced as if method_setImplementation(_:_:) were called. The type encoding specified by `types` is ignored.

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

