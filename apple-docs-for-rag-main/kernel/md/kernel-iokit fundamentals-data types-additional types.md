

- Kernel
- IOKit Fundamentals
- Data Types
-  Additional Types 

API Collection

# Additional Types

Find custom type definitions and pointer types for standard classes.

## Topics

### Pointers

OSArrayPtr

OSBooleanPtr

OSCollectionIteratorPtr

OSCollectionPtr

OSDataConstPtr

OSDataPtr

OSDictionaryPtr

OSNumberPtr

OSOrderedSetPtr

OSSerializePtr

OSSerializerPtr

OSSetPtr

OSStringConstPtr

OSStringPtr

OSSymbolConstPtr

OSSymbolPtr

OSTypePtr

### Structures

OSClassDescription

OSMallocTag

An opaque type used to track memory allocations.

OSMallocTag_t

See OSMallocTag.

OSNotificationHeader64

### Typedefs

OSAsyncReference

OSAsyncReference64

OSContainer

OSKextRequestTag

Identifies a kext request made to user space.

OSIterator

OSType

## See Also

### Base Types

OSSymbol

OSSymbol wraps a C string in a unique C++ object for use as keys in Libkern collections.

OSObject

OSObject is the concrete root class of the Libkern and I/O Kit C++ class hierarchy.

OSMetaClass

OSMetaClassBase

OSMetaClassBase is the abstract bootstrap class for the Libkern and I/O Kit run-time type information system.

OSObjectPtr

OSObjectRef

