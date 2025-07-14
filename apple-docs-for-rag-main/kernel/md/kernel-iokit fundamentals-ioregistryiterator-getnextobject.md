

- Kernel
- IOKit Fundamentals
- IORegistryIterator
-  getNextObject 

# getNextObject

Return the next object in the registry iteration.

``` source
virtual IORegistryEntry * getNextObject(
 void ); 
```

## Return Value

The next registry entry in the iteration (the current entry), or zero if the iteration has finished at this level of recursion. The entry returned is retained while the iterator is pointing at it (its the current entry), or recursing into it. The caller should not release it.

## Overview

This method calls either getNextObjectFlat or getNextObjectRecursive depending on the options the iterator was created with. This implements the OSIterator defined getNextObject method. The object returned is retained while the iterator is pointing at it (its the current entry), or recursing into it. The caller should not release it.

## See Also

### Miscellaneous

enterEntry()

Recurse into the current entry in the registry iteration.

enterEntry(const IORegistryPlane *)

Recurse into the current entry in the registry iteration.

exitEntry

Exits a level of recursion, restoring the current entry.

getCurrentEntry

Return the current entry in the registry iteration.

getNextObjectFlat

Return the next object in the registry iteration, ignoring the kIORegistryIterateRecursively option.

getNextObjectRecursive

Return the next object in the registry iteration, and enter it.

isValid

Checks that no registry changes have invalidated the iteration.

iterateAll

Iterates all entries (with getNextObject) and returns a set of all returned entries.

iterateOver(const IORegistryPlane *, IOOptionBits)

Create an iterator rooted at the registry root.

iterateOver(IORegistryEntry *, const IORegistryPlane *, IOOptionBits)

Create an iterator rooted at a given registry entry.

reset

Exits all levels of recursion, restoring the iterator to its state at creation.

