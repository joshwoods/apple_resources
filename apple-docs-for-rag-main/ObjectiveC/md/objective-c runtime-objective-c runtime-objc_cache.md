

- Objective-C Runtime
- Objective-C Runtime
-  objc_cache 

# objc_cache

Performance optimization for method calls. Contains pointers to recently used methods.

## Overview

To limit the need to perform linear searches of method lists for the definitions of frequently accessed methods—an operation that can considerably slow down method lookup—the Objective-C runtime functions store pointers to the definitions of the most recently called method of the class in an `objc_cache` data structure.

## Topics

### Fields

mask

An integer specifying the total number of allocated cache buckets (minus one). During method lookup, the Objective-C runtime uses this field to determine the index at which to begin a linear search of the `buckets` array. A pointer to a method’s selector is masked against this field using a logical AND operation (`index = (mask & selector))`. This serves as a simple hashing algorithm.

occupied

An integer specifying the total number of occupied cache buckets.

buckets

An array of pointers to Method data structures. This array may contain no more than `mask + 1` items. Note that pointers may be `NULL`, indicating that the cache bucket is unoccupied, and occupied buckets may not be contiguous. This array may grow over time.

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

struct objc_property_attribute_t

Defines a property attribute.

