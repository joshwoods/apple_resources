

- Kernel
- IOKit Fundamentals
- Data Types
-  OSMetaClassBase 

Class

# OSMetaClassBase

OSMetaClassBase is the abstract bootstrap class for the Libkern and I/O Kit run-time type information system.

macOS 10.0+

``` source
class OSMetaClassBase
```

## Overview

OSMetaClassBase is the abstract C++ root class underlying the entire Libkern and I/O Kit class hierarchy. It defines the run-time type information system, including dynamic class allocation and safe type-casting, as well as the abstract interface for reference counting and a few other utility functions. OSMetaClassBase is the immediate superclass of OSObject and OSMetaClass; no other class should derive from OSMetaClassBase.

For more information, see Introduction to I/O Kit Device Driver Design Guidelines.

**Use by Kernel Extensions**

Kernel Extensions should never interact directly with OSMetaClassBase, but they will find useful several macros that tie in to the run-time type information system, specifically:

- OSTypeAlloc - allocation of new instances

- OSDynamicCast - safe type casting

- OSCheckTypeInst - checking for inheritance/derivation

- OSMemberFunctionCast - casting C++ member functions to C function pointers for registration as callbacks

See OSMetaClass for more run-time type information interfaces.

**Use Restrictions**

OSMetaClassBase should not be subclassed by kernel extensions, nor should kernel extensions call its run-time type functions directly.

The run-time type functions and macros are **not safe** to call in a primary interrupt context.

**Concurrency Protection**

The run-time type macros and functions of OSMetaClassBase are thread-safe.

## Topics

### Miscellaneous

OSCheckTypeInst

Checks whether two objects are type-compatible.

OSDynamicCast

OSMemberFunctionCast

Converts a C++ member function pointer, relative to an instance, to a C-style pointer to function.

OSSafeRelease

Release an object if not `NULL`.

OSSafeReleaseNULL

OSTypeAlloc

OSTypeID

OSTypeIDInst

checkTypeInst

Checks whether an object instance is of the same class as another object instance (or a subclass of that class).

getMetaClass

Returns the OSMetaClass representing an OSMetaClassBase subclass.

getRetainCount

Abstract declaration of getRetainCount().

isEqualTo

Checks whether another object is equal to the receiver.

metaCast(const char *)

Casts this object is to the class managed by the named OSMetaClass.

metaCast(const OSMetaClass *)

Casts this object is to the class managed by the given OSMetaClass.

metaCast(const OSString *)

Casts this object is to the class managed by the named OSMetaClass.

metaCast(const OSSymbol *)

Casts this object is to the class managed by the named OSMetaClass.

release()

Abstract declaration of release.

release(int)

Abstract declaration of release(int freeWhen).

retain

Abstract declaration of retain().

safeMetaCast

Casts an object is to the class managed by the given OSMetaClass.

serialize

Abstract declaration of serialize.

taggedRelease(const void *)

Abstract declaration of taggedRelease(const void \*).

taggedRelease(const void *, const int)

Abstract declaration of taggedRelease(const void \*, const int freeWhen).

taggedRetain

Abstract declaration of taggedRetain(const void \*).

### Instance Methods

- Dispatch

Runtime internals

- Invoke

Runtime internals

- getMetaClass

- getRetainCount

- isEqualTo

- metaCast

- metaCast

- metaCast

- metaCast

- operator=

- release

- release

- retain

- serialize

- taggedRelease

- taggedRelease

- taggedRetain

### Type Methods

+ checkTypeInst

+ initialize

+ requiredMetaCast

+ safeMetaCast

## See Also

### Base Types

OSSymbol

OSSymbol wraps a C string in a unique C++ object for use as keys in Libkern collections.

OSObject

OSObject is the concrete root class of the Libkern and I/O Kit C++ class hierarchy.

OSMetaClass

OSObjectPtr

OSObjectRef

Additional Types

Find custom type definitions and pointer types for standard classes.

