

- Kernel
- IOKit Fundamentals
- IORegistryIterator
-  iterateAll 

# iterateAll

Iterates all entries (with getNextObject) and returns a set of all returned entries.

``` source
virtual OSOrderedSet * iterateAll(
 void ); 
```

## Return Value

A set of entries returned by the iteration. The caller should release the set when it has finished with it. Zero is returned on a resource failure.

## Overview

This method will reset, then iterate all entries in the iteration (with getNextObject) until successful (ie. the iterator is valid at the end of the iteration).

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

isValid

Checks that no registry changes have invalidated the iteration.

iterateOver(const IORegistryPlane *, IOOptionBits)

Create an iterator rooted at the registry root.

iterateOver(IORegistryEntry *, const IORegistryPlane *, IOOptionBits)

Create an iterator rooted at a given registry entry.

reset

Exits all levels of recursion, restoring the iterator to its state at creation.

