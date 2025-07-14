

- Objective-C Runtime
-  IMP 

Type Alias

# IMP

A pointer to the start of a method implementation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias IMP = OpaquePointer
```

## Discussion

This data type is a pointer to the start of the function that implements the method. This function uses standard C calling conventions as implemented for the current CPU architecture. The first argument is a pointer to `self` (that is, the memory for the particular instance of this class, or, for a class method, a pointer to the metaclass). The second argument is the method selector. The method arguments follow.

## See Also

### Class-Definition Data Structures

typealias Method

An opaque type that represents a method in a class definition.

typealias Ivar

An opaque type that represents an instance variable.

typealias Category

An opaque type that represents a category.

typealias objc_property_t

An opaque type that represents an Objective-C declared property.

struct objc_method_description

Defines an Objective-C method.

objc_cache

Performance optimization for method calls. Contains pointers to recently used methods.

struct objc_property_attribute_t

Defines a property attribute.

