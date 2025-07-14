

- Kernel
- IOKit Fundamentals
- Data Types
- OSSymbol
-  isEqualTo(const OSSymbol \*) 

# isEqualTo(const OSSymbol \*)

Tests the equality of two OSSymbol objects.

``` source
virtual bool isEqualTo(
 const OSSymbol *aSymbol) const; 
```

## Parameters 

`aSymbol`  

The OSSymbol object being compared against the receiver.

## Return Value

`true` if the two OSSymbol objects are equivalent, `false` otherwise.

## Overview

Two OSSymbol objects are considered equal if they have the same address; that is, this function is equivalent to the `==` operator.

## See Also

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

