

- Kernel
- IOKit Fundamentals
- Data Types
- OSSymbol
-  withString 

# withString

Returns an OSSymbol created from an OSString, or the existing unique instance of the same value.

``` source
static const OSSymbol * withString(
 const OSString *aString); 
```

## Parameters 

`aString`  

The OSString object to look up or copy.

## Return Value

An instance of OSSymbol representing the same characters as `aString`; `NULL` on failure.

## Overview

This function creates or returns the unique OSSymbol instance representing the string value of `aString`. You can compare it with other OSSymbols using the `==` operator.

OSSymbols are reference-counted normally. This function either returns a new OSSymbol with a retain count of 1, or increments the retain count of the existing instance.

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

