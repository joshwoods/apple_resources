

- Kernel
- IOKit Fundamentals
- Data Types
- OSSymbol
-  taggedRelease(const void \*, const int) 

# taggedRelease(const void \*, const int)

Overrides OSObject::taggedRelease(const void \*, const int) to synchronize with the symbol pool.

``` source
virtual void taggedRelease( 
 const void *tag, 
 const intfreeWhen) const; 
```

## Parameters 

`tag`  

Used for tracking collection references.

`freeWhen`  

If decrementing the reference count makes it \>= `freeWhen`, the object is immediately freed.

## Overview

Because OSSymbol shares instances, the reference-counting functions must synchronize access to the class-internal tables used to track those instances.

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

withCString

Returns an OSSymbol created from a C string, or the existing unique instance of the same value.

withCStringNoCopy

Returns an OSSymbol created from a C string, without copying that string, or the existing unique instance of the same value.

withString

Returns an OSSymbol created from an OSString, or the existing unique instance of the same value.

