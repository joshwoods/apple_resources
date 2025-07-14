

- Objective-C Runtime
-  NXHashTablePrototype 

Structure

# NXHashTablePrototype

Mac CatalystmacOS

``` source
struct NXHashTablePrototype
```

## Topics

### Initializers

init(hash: (UnsafeRawPointer?, UnsafeRawPointer?) -> UInt, isEqual: (UnsafeRawPointer?, UnsafeRawPointer?, UnsafeRawPointer?) -> Int32, free: (UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void, style: Int32)

### Instance Properties

var free: (UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void

var hash: (UnsafeRawPointer?, UnsafeRawPointer?) -> UInt

var isEqual: (UnsafeRawPointer?, UnsafeRawPointer?, UnsafeRawPointer?) -> Int32

var style: Int32

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Structures

struct NSZone

struct ObjCBool

struct ObjCClassList

struct Selector

struct objc_method_description

Defines an Objective-C method.

struct objc_object

Represents an instance of a class.

struct objc_property_attribute_t

Defines a property attribute.

struct objc_super

Specifies the superclass of an instance.

