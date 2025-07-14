

- Kernel
- IOKit Fundamentals
- Data Types
-  OSSymbol 

Class

# OSSymbol

OSSymbol wraps a C string in a unique C++ object for use as keys in Libkern collections.

macOS 10.0+

``` source
class OSSymbol : OSString
```

## Overview

OSSymbol is a container class for managing uniqued strings, for example, those used as dictionary keys. Its static instance-creation functions check for an existing instance of OSSymbol with the requested C string value before creating a new object. If an instance already exists in the pool of unique symbols, its reference count is incremented and the existing instance is returned.

While OSSymbol provides for uniquing of a given string value, it makes no effort to enforce immutability of that value. Altering the contents of an OSSymbol should be avoided.

**Use Restrictions**

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are **unsafe** to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

OSSymbol provides no concurrency protection; it's up to the usage context to provide any protection necessary. Some portions of the I/O Kit, such as IORegistryEntry, handle synchronization via defined member functions for setting properties.

## Topics

### Miscellaneous

free

Overrides OSObject::free to synchronize with the symbol pool.

initWithCString

Overridden to prevent creation of duplicate symbols.

initWithCStringNoCopy

Overridden to prevent creation of duplicate symbols.

initWithString

Overridden to prevent creation of duplicate symbols.

isEqualTo

Tests the equality of an OSSymbol object to an arbitrary object.

isEqualTo(const char *)

Tests the equality of an OSSymbol object with a C string.

isEqualTo(const OSSymbol *)

Tests the equality of two OSSymbol objects.

taggedRelease(const void *)

Overrides OSObject::taggedRelease(const void \*) to synchronize with the symbol pool.

taggedRelease(const void *, const int)

Overrides OSObject::taggedRelease(const void \*, const int) to synchronize with the symbol pool.

withCString

Returns an OSSymbol created from a C string, or the existing unique instance of the same value.

withCStringNoCopy

Returns an OSSymbol created from a C string, without copying that string, or the existing unique instance of the same value.

withString

Returns an OSSymbol created from an OSString, or the existing unique instance of the same value.

### Instance Methods

- free

- getMetaClass

- initWithCString

- initWithCStringNoCopy

- initWithString

- isEqualTo

- isEqualTo

- isEqualTo

- taggedRelease

- taggedRelease

- taggedRetain

### Type Methods

+ existingSymbolForCString

+ existingSymbolForString

+ initialize

+ withCString

+ withCStringNoCopy

+ withString

## Relationships

### Inherits From

- OSString

## See Also

### Base Types

OSObject

OSObject is the concrete root class of the Libkern and I/O Kit C++ class hierarchy.

OSMetaClass

OSMetaClassBase

OSMetaClassBase is the abstract bootstrap class for the Libkern and I/O Kit run-time type information system.

OSObjectPtr

OSObjectRef

Additional Types

Find custom type definitions and pointer types for standard classes.

