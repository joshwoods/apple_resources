

- Kernel
- IOKit Fundamentals
- Data Types
- OSSymbol
-  isEqualTo(const char \*) 

# isEqualTo(const char \*)

Tests the equality of an OSSymbol object with a C string.

``` source
virtual bool isEqualTo(
 const char *cString) const; 
```

## Parameters 

`cString`  

The C string to compare against the receiver.

## Return Value

`true` if the OSSymbol's characters are equivalent to the C string's, `false` otherwise.

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

