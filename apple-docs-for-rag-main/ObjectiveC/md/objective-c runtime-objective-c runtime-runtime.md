

- Objective-C Runtime
-  Objective-C Runtime 

API Collection

# Objective-C Runtime

Describes the macOS Objective-C runtime library support functions and data structures.

## Overview

The Objective-C runtime is a runtime library that provides support for the dynamic properties of the Objective-C language, and as such is linked to by all Objective-C apps. Objective-C runtime library support functions are implemented in the shared library found at `/usr/lib/libobjc.A.dylib`.

You typically don’t need to use the Objective-C runtime library directly when programming in Objective-C. This API is useful primarily for developing bridge layers between Objective-C and other languages, or for low-level debugging.

The macOS implementation of the Objective-C runtime library is unique to the Mac. For other platforms, the GNU Compiler Collection provides a different implementation with a similar API. This document covers only the macOS implementation.

The low-level Objective-C runtime API is significantly updated in OS X version 10.5. Many functions and all existing data structures are replaced with new functions. The old functions and structures are deprecated in 32-bit and absent in 64-bit mode. The API constrains several values to 32-bit ints even in 64-bit mode—class count, protocol count, methods per class, ivars per class, arguments per method, sizeof(all arguments) per method, and class version number. In addition, the new Objective-C ABI (not described here) further constrains `sizeof(anInstance)` to 32 bits, and three other values to 24 bits—methods per class, ivars per class, and sizeof(a single ivar). Finally, the obsolete `NXHashTable` and `NXMapTable` are limited to 4 billion items.

String encoding

All `char *` in the runtime API should be considered to have UTF-8 encoding.

“Deprecated” below means “deprecated in OS X version 10.5 for 32-bit code, and disallowed for 64-bit code.”

### Who Should Read This Document

The document is intended for readers who might be interested in learning about the Objective-C runtime.

Because this isn’t a document about C, it assumes some prior acquaintance with that language. However, it doesn’t have to be an extensive acquaintance.

## Topics

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

func class_addMethod(AnyClass?, Selector, IMP, UnsafePointer&lt;CChar>?) -> Bool

Adds a new method to a class with a given name and implementation.

func class_getInstanceMethod(AnyClass?, Selector) -> Method?

Returns a specified instance method for a given class.

func class_getClassMethod(AnyClass?, Selector) -> Method?

Returns a pointer to the data structure describing a given class method for a given class.

func class_copyMethodList(AnyClass?, UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;Method>?

Describes the instance methods implemented by a class.

func class_replaceMethod(AnyClass?, Selector, IMP, UnsafePointer&lt;CChar>?) -> IMP?

Replaces the implementation of a method for a given class.

func class_getMethodImplementation(AnyClass?, Selector) -> IMP?

Returns the function pointer that would be called if a particular message were sent to an instance of a class.

func class_getMethodImplementation_stret(AnyClass?, Selector) -> IMP?

Returns the function pointer that would be called if a particular message were sent to an instance of a class.

func class_respondsToSelector(AnyClass?, Selector) -> Bool

Returns a Boolean value that indicates whether instances of a class respond to a particular selector.

func class_addProtocol(AnyClass?, Protocol) -> Bool

Adds a protocol to a class.

func class_addProperty(AnyClass?, UnsafePointer&lt;CChar>, UnsafePointer&lt;objc_property_attribute_t>?, UInt32) -> Bool

Adds a property to a class.

func class_replaceProperty(AnyClass?, UnsafePointer&lt;CChar>, UnsafePointer&lt;objc_property_attribute_t>?, UInt32)

Replace a property of a class.

func class_conformsToProtocol(AnyClass?, Protocol?) -> Bool

Returns a Boolean value that indicates whether a class conforms to a given protocol.

func class_copyProtocolList(AnyClass?, UnsafeMutablePointer&lt;UInt32>?) -> AutoreleasingUnsafeMutablePointer&lt;Protocol>?

Describes the protocols adopted by a class.

func class_getVersion(AnyClass?) -> Int32

Returns the version number of a class definition.

func class_setVersion(AnyClass?, Int32)

Sets the version number of a class definition.

objc_setFutureClass

Used by CoreFoundation’s toll-free bridging.

### Adding Classes

func objc_allocateClassPair(AnyClass?, UnsafePointer&lt;CChar>, Int) -> AnyClass?

Creates a new class and metaclass.

func objc_disposeClassPair(AnyClass)

Destroys a class and its associated metaclass.

func objc_registerClassPair(AnyClass)

Registers a class that was allocated using objc_allocateClassPair(_:_:_:).

func objc_duplicateClass(AnyClass, UnsafePointer&lt;CChar>, Int) -> AnyClass

Used by Foundation’s Key-Value Observing.

### Instantiating Classes

func class_createInstance(AnyClass?, Int) -> Any?

Creates an instance of a class, allocating memory for the class in the default malloc memory zone.

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

func object_setClass(Any?, AnyClass) -> AnyClass?

Sets the class of an object.

### Obtaining Class Definitions

func objc_getClassList(AutoreleasingUnsafeMutablePointer&lt;AnyClass>?, Int32) -> Int32

Obtains the list of registered class definitions.

func objc_copyClassList(UnsafeMutablePointer&lt;UInt32>?) -> AutoreleasingUnsafeMutablePointer&lt;AnyClass>?

Creates and returns a list of pointers to all registered class definitions.

func objc_lookUpClass(UnsafePointer&lt;CChar>) -> AnyClass?

Returns the class definition of a specified class.

func objc_getClass(UnsafePointer&lt;CChar>) -> Any!

Returns the class definition of a specified class.

func objc_getRequiredClass(UnsafePointer&lt;CChar>) -> AnyClass

Returns the class definition of a specified class.

func objc_getMetaClass(UnsafePointer&lt;CChar>) -> Any!

Returns the metaclass definition of a specified class.

### Working with Instance Variables

func ivar_getName(Ivar) -> UnsafePointer&lt;CChar>?

Returns the name of an instance variable.

func ivar_getTypeEncoding(Ivar) -> UnsafePointer&lt;CChar>?

Returns the type string of an instance variable.

func ivar_getOffset(Ivar) -> Int

Returns the offset of an instance variable.

### Associative References

func objc_setAssociatedObject(Any, UnsafeRawPointer, Any?, objc_AssociationPolicy)

Sets an associated value for a given object using a given key and association policy.

func objc_getAssociatedObject(Any, UnsafeRawPointer) -> Any?

Returns the value associated with a given object for a given key.

func objc_removeAssociatedObjects(Any)

Removes all associations for a given object.

### Working with Methods

func method_getName(Method) -> Selector

Returns the name of a method.

func method_getImplementation(Method) -> IMP

Returns the implementation of a method.

func method_getTypeEncoding(Method) -> UnsafePointer&lt;CChar>?

Returns a string describing a method’s parameter and return types.

func method_copyReturnType(Method) -> UnsafeMutablePointer&lt;CChar>

Returns a string describing a method’s return type.

func method_copyArgumentType(Method, UInt32) -> UnsafeMutablePointer&lt;CChar>?

Returns a string describing a single parameter type of a method.

func method_getReturnType(Method, UnsafeMutablePointer&lt;CChar>, Int)

Returns by reference a string describing a method’s return type.

func method_getNumberOfArguments(Method) -> UInt32

Returns the number of arguments accepted by a method.

func method_getArgumentType(Method, UInt32, UnsafeMutablePointer&lt;CChar>?, Int)

Returns by reference a string describing a single parameter type of a method.

func method_getDescription(Method) -> UnsafeMutablePointer&lt;objc_method_description>

Returns a method description structure for a specified method.

func method_setImplementation(Method, IMP) -> IMP

Sets the implementation of a method.

func method_exchangeImplementations(Method, Method)

Exchanges the implementations of two methods.

### Working with Libraries

func objc_copyImageNames(UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>>

Returns the names of all the loaded Objective-C frameworks and dynamic libraries.

func class_getImageName(AnyClass?) -> UnsafePointer&lt;CChar>?

Returns the name of the dynamic library a class originated from.

func objc_copyClassNamesForImage(UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>>?

Returns the names of all the classes within a specified library or framework.

### Working with Selectors

func sel_getName(Selector) -> UnsafePointer&lt;CChar>

Returns the name of the method specified by a given selector.

func sel_registerName(UnsafePointer&lt;CChar>) -> Selector

Registers a method with the Objective-C runtime system, maps the method name to a selector, and returns the selector value.

func sel_getUid(UnsafePointer&lt;CChar>) -> Selector

Registers a method name with the Objective-C runtime system.

func sel_isEqual(Selector, Selector) -> Bool

Returns a Boolean value that indicates whether two selectors are equal.

### Working with Protocols

func objc_getProtocol(UnsafePointer&lt;CChar>) -> Protocol?

Returns a specified protocol.

func objc_copyProtocolList(UnsafeMutablePointer&lt;UInt32>?) -> AutoreleasingUnsafeMutablePointer&lt;Protocol>?

Returns an array of all the protocols known to the runtime.

func objc_allocateProtocol(UnsafePointer&lt;CChar>) -> Protocol?

Creates a new protocol instance.

func objc_registerProtocol(Protocol)

Registers a newly created protocol with the Objective-C runtime.

func protocol_addMethodDescription(Protocol, Selector, UnsafePointer&lt;CChar>?, Bool, Bool)

Adds a method to a protocol.

func protocol_addProtocol(Protocol, Protocol)

Adds a registered protocol to another protocol that is under construction.

func protocol_addProperty(Protocol, UnsafePointer&lt;CChar>, UnsafePointer&lt;objc_property_attribute_t>?, UInt32, Bool, Bool)

Adds a property to a protocol that is under construction.

func protocol_getName(Protocol) -> UnsafePointer&lt;CChar>

Returns the name of a protocol.

func protocol_isEqual(Protocol?, Protocol?) -> Bool

Returns a Boolean value that indicates whether two protocols are equal.

func protocol_copyMethodDescriptionList(Protocol, Bool, Bool, UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;objc_method_description>?

Returns an array of method descriptions of methods meeting a given specification for a given protocol.

func protocol_getMethodDescription(Protocol, Selector, Bool, Bool) -> objc_method_description

Returns a method description structure for a specified method of a given protocol.

func protocol_copyPropertyList(Protocol, UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;objc_property_t>?

Returns an array of the properties declared by a protocol.

func protocol_getProperty(Protocol, UnsafePointer&lt;CChar>, Bool, Bool) -> objc_property_t?

Returns the specified property of a given protocol.

func protocol_copyProtocolList(Protocol, UnsafeMutablePointer&lt;UInt32>?) -> AutoreleasingUnsafeMutablePointer&lt;Protocol>?

Returns an array of the protocols adopted by a protocol.

func protocol_conformsToProtocol(Protocol?, Protocol?) -> Bool

Returns a Boolean value that indicates whether one protocol conforms to another protocol.

### Working with Properties

func property_getName(objc_property_t) -> UnsafePointer&lt;CChar>

Returns the name of a property.

func property_getAttributes(objc_property_t) -> UnsafePointer&lt;CChar>?

Returns the attribute string of a property.

func property_copyAttributeValue(objc_property_t, UnsafePointer&lt;CChar>) -> UnsafeMutablePointer&lt;CChar>?

Returns the value of a property attribute given the attribute name.

func property_copyAttributeList(objc_property_t, UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;objc_property_attribute_t>?

Returns an array of property attributes for a given property.

### Using Objective-C Language Features

func objc_enumerationMutation(Any)

Inserted by the compiler when a mutation is detected during a foreach iteration.

func objc_setEnumerationMutationHandler(((Any) -> Void)?)

Sets the current mutation handler.

func imp_implementationWithBlock(Any) -> IMP

Creates a pointer to a function that calls the specified block when the method is called.

func imp_getBlock(IMP) -> Any?

Returns the block associated with an `IMP` that was created using imp_implementationWithBlock(_:).

func imp_removeBlock(IMP) -> Bool

Disassociates a block from an `IMP` that was created using imp_implementationWithBlock(_:), and releases the copy of the block that was created.

func objc_loadWeak(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>) -> Any?

Loads the object referenced by a weak pointer and returns it.

func objc_storeWeak(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, Any?) -> Any?

Stores a new value in a `__weak` variable.

### Class-Definition Data Structures

typealias Method

An opaque type that represents a method in a class definition.

typealias Ivar

An opaque type that represents an instance variable.

typealias Category

An opaque type that represents a category.

typealias objc_property_t

An opaque type that represents an Objective-C declared property.

typealias IMP

A pointer to the start of a method implementation.

struct objc_method_description

Defines an Objective-C method.

objc_cache

Performance optimization for method calls. Contains pointers to recently used methods.

struct objc_property_attribute_t

Defines a property attribute.

### Instance Data Types

These are the data types that represent objects, classes, and superclasses.

struct objc_object

Represents an instance of a class.

struct objc_super

Specifies the superclass of an instance.

### Associative References

enum objc_AssociationPolicy

Type to specify the behavior of an association.

## See Also

### Related Documentation

Objective-C Runtime Programming Guide

### Reference

Objective-C Structures

Objective-C Constants

Objective-C Functions

Objective-C Data Types

Objective-C Macros

Objective-C Enumerations

