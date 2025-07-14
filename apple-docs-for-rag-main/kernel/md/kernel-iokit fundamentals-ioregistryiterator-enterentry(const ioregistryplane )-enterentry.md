

- Kernel
- IOKit Fundamentals
- IORegistryIterator
-  enterEntry(const IORegistryPlane \*) 

# enterEntry(const IORegistryPlane \*)

Recurse into the current entry in the registry iteration.

``` source
virtual void enterEntry(
 const IORegistryPlane *plane ); 
```

## Parameters 

`plane`  

The new plane to switch into.

## Overview

This method recurses into an entry as with enterEntry, but also switches from the current plane to a new one set by the caller.

## See Also

### Miscellaneous

enterEntry()

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

iterateAll

Iterates all entries (with getNextObject) and returns a set of all returned entries.

iterateOver(const IORegistryPlane *, IOOptionBits)

Create an iterator rooted at the registry root.

iterateOver(IORegistryEntry *, const IORegistryPlane *, IOOptionBits)

Create an iterator rooted at a given registry entry.

reset

Exits all levels of recursion, restoring the iterator to its state at creation.

