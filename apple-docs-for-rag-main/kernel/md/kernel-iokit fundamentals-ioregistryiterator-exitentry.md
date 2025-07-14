

- Kernel
- IOKit Fundamentals
- IORegistryIterator
-  exitEntry 

# exitEntry

Exits a level of recursion, restoring the current entry.

``` source
virtual bool exitEntry(
 void ); 
```

## Return Value

true if a level of recursion was undone, false if no recursive levels are left in the iteration.

## Overview

This method undoes an enterEntry, restoring the current entry. If there are no more levels of recursion to exit false is returned, otherwise true is returned.

## See Also

### Miscellaneous

enterEntry()

Recurse into the current entry in the registry iteration.

enterEntry(const IORegistryPlane *)

Recurse into the current entry in the registry iteration.

getCurrentEntry

Return the current entry in the registry iteration.

getNextObject

Return the next object in the registry iteration.

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

