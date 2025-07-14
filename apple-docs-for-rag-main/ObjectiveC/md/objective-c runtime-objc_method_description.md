

- Objective-C Runtime
-  objc_method_description 

Structure

# objc_method_description

Defines an Objective-C method.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct objc_method_description
```

## Topics

### Fields

var name: Selector?

The name of the method at runtime.

var types: UnsafeMutablePointer&lt;CChar>?

The types of the method arguments.

### Initializers

init()

init(name: Selector?, types: UnsafeMutablePointer&lt;CChar>?)

## Relationships

### Conforms To

- BitwiseCopyable

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

typealias IMP

A pointer to the start of a method implementation.

objc_cache

Performance optimization for method calls. Contains pointers to recently used methods.

struct objc_property_attribute_t

Defines a property attribute.

