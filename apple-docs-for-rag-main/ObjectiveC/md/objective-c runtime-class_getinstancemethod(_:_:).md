

- Objective-C Runtime
-  class_getInstanceMethod(\_:\_:) 

Function

# class_getInstanceMethod(\_:\_:)

Returns a specified instance method for a given class.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func class_getInstanceMethod(
    _ cls: AnyClass?,
    _ name: Selector
) -> Method?
```

## Parameters 

`cls`  

The class you want to inspect.

`name`  

The selector of the method you want to retrieve.

## Return Value

The method that corresponds to the implementation of the selector specified by `aSelector` for the class specified by `aClass`, or `NULL` if the specified class or its superclasses do not contain an instance method with the specified selector.

## Discussion

Note that this function searches superclasses for implementations, whereas class_copyMethodList(_:_:) does not.

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

