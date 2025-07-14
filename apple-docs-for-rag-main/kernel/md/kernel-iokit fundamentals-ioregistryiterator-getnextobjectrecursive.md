

- Kernel
- IOKit Fundamentals
- IORegistryIterator
-  getNextObjectRecursive 

# getNextObjectRecursive

Return the next object in the registry iteration, and enter it.

``` source
virtual IORegistryEntry * getNextObjectRecursive(
 void ); 
```

## Return Value

The next registry entry in the iteration (the current entry), or zero if its finished, or the iteration is invalid (see isValid). The entry returned is retained while the iterator is pointing at it (its the current entry), or recursing into it. The caller should not release it.

## Overview

If the iterator has a current entry, and the iterator has not already entered previously, enterEntry is called to recurse into it, ie. make it the new root, and the next child, or parent if the kIORegistryIterateParents option was used to create the iterator, at this new level of recursion is returned. If there is no current entry at this level of recursion, exitEntry is called and the process repeats, until the iteration returns to the entry the iterator was created with and zero is returned. The object returned is retained while the iterator is pointing at it (its the current entry), or recursing into it. The caller should not release it.

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

