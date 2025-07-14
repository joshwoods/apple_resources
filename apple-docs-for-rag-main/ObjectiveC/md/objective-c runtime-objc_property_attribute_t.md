

- Objective-C Runtime
-  objc_property_attribute_t 

Structure

# objc_property_attribute_t

Defines a property attribute.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct objc_property_attribute_t
```

## Topics

### Initializers

init(name: UnsafePointer&lt;CChar>, value: UnsafePointer&lt;CChar>)

### Instance Properties

var name: UnsafePointer&lt;CChar>

The name of the attribute.

var value: UnsafePointer&lt;CChar>

The value of the attribute (usually empty).

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

struct objc_method_description

Defines an Objective-C method.

objc_cache

Performance optimization for method calls. Contains pointers to recently used methods.

