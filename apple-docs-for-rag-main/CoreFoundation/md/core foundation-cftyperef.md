

- Core Foundation
-  CFTypeRef 

Type Alias

# CFTypeRef

An untyped “generic” reference to any Core Foundation object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFTypeRef = AnyObject
```

## Discussion

All other Core Foundation opaque types derive from `CFTypeRef`. The functions, callbacks, data types, and constants defined for CFType can be used by any derived opaque type. Hence, `CFTypeRef` functions are referred to as “polymorphic functions.” You use `CFTypeRef` functions to retain and release objects, to compare and inspect objects, get descriptions of objects and opaque types, and to get object allocators.

## Topics

### Memory Management

func CFGetAllocator(CFTypeRef!) -> CFAllocator!

Returns the allocator used to allocate a Core Foundation object.

func CFGetRetainCount(CFTypeRef!) -> CFIndex

Returns the reference count of a Core Foundation object.

### Determining Equality

func CFEqual(CFTypeRef!, CFTypeRef!) -> Bool

Determines whether two Core Foundation objects are considered equal.

### Hashing

func CFHash(CFTypeRef!) -> CFHashCode

Returns a code that can be used to identify an object in a hashing structure.

### Miscellaneous Functions

func CFCopyDescription(CFTypeRef!) -> CFString!

Returns a textual description of a Core Foundation object.

func CFCopyTypeIDDescription(CFTypeID) -> CFString!

Returns a textual description of a Core Foundation type, as identified by its type ID, which can be used when debugging.

func CFGetTypeID(CFTypeRef!) -> CFTypeID

Returns the unique identifier of an opaque type to which a Core Foundation object belongs.

func CFShow(CFTypeRef!)

Prints a description of a Core Foundation object to stderr.

### Data Types

typealias CFHashCode

A type for hash codes returned by the `CFHash` function.

typealias CFTypeID

A type for unique, constant integer values that identify particular Core Foundation opaque types.

## See Also

### Related Documentation

Memory Management Programming Guide for Core Foundation

Core Foundation Design Concepts

### Data Types

typealias CFAllocatorTypeID

struct CFCalendarIdentifier

struct CFDateFormatterKey

typealias CFErrorDomain

struct CFLocaleIdentifier

struct CFLocaleKey

struct CFNotificationName

struct CFNumberFormatterKey

struct CFRunLoopMode

struct CFStreamPropertyKey

