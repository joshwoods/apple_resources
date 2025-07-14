

- Kernel
- IOKit Fundamentals
- IORegistryIterator
-  isValid 

# isValid

Checks that no registry changes have invalidated the iteration.

``` source
virtual bool isValid(
 void ); 
```

## Return Value

false if the iterator has been invalidated by changes to the registry, true otherwise.

## Overview

If a registry iteration is invalidated by changes to the registry, it will be made invalid, the currentEntry will be considered zero, and further calls to getNextObject et al. will return zero. The iterator should be reset to restart the iteration when this happens.

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

getNextObject

Return the next object in the registry iteration.

getNextObjectFlat

Return the next object in the registry iteration, ignoring the kIORegistryIterateRecursively option.

getNextObjectRecursive

Return the next object in the registry iteration, and enter it.

iterateAll

Iterates all entries (with getNextObject) and returns a set of all returned entries.

iterateOver(const IORegistryPlane *, IOOptionBits)

Create an iterator rooted at the registry root.

iterateOver(IORegistryEntry *, const IORegistryPlane *, IOOptionBits)

Create an iterator rooted at a given registry entry.

reset

Exits all levels of recursion, restoring the iterator to its state at creation.

