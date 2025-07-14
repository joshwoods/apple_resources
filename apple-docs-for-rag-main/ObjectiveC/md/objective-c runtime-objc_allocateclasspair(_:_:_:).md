

- Objective-C Runtime
-  objc_allocateClassPair(\_:\_:\_:) 

Function

# objc_allocateClassPair(\_:\_:\_:)

Creates a new class and metaclass.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_allocateClassPair(
    _ superclass: AnyClass?,
    _ name: UnsafePointer,
    _ extraBytes: Int
) -> AnyClass?
```

## Parameters 

`superclass`  

The class to use as the new class’s superclass, or `Nil` to create a new root class.

`name`  

The string to use as the new class’s name. The string will be copied.

`extraBytes`  

The number of bytes to allocate for indexed ivars at the end of the class and metaclass objects. This should usually be `0`.

## Return Value

The new class, or `Nil` if the class could not be created (for example, the desired name is already in use).

## Discussion

You can get a pointer to the new metaclass by calling `object_getClass(newClass)`.

To create a new class, start by calling objc_allocateClassPair(_:_:_:). Then set the class’s attributes with functions like class_addMethod(_:_:_:_:) and class_addIvar(_:_:_:_:_:). When you are done building the class, call objc_registerClassPair(_:). The new class is now ready for use.

Instance methods and instance variables should be added to the class itself. Class methods should be added to the metaclass.

## See Also

### Adding Classes

func objc_disposeClassPair(AnyClass)

Destroys a class and its associated metaclass.

func objc_registerClassPair(AnyClass)

Registers a class that was allocated using objc_allocateClassPair(_:_:_:).

func objc_duplicateClass(AnyClass, UnsafePointer&lt;CChar>, Int) -> AnyClass

Used by Foundation’s Key-Value Observing.

