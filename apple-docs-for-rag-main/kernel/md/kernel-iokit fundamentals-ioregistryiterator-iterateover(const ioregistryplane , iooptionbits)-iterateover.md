

- Kernel
- IOKit Fundamentals
- IORegistryIterator
-  iterateOver(const IORegistryPlane \*, IOOptionBits) 

# iterateOver(const IORegistryPlane \*, IOOptionBits)

Create an iterator rooted at the registry root.

``` source
static IORegistryIterator * iterateOver(
 const IORegistryPlane *plane, 
 IOOptionBits options = 0 ); 
```

## Parameters 

`plane`  

A plane object must be specified.

`options`  

kIORegistryIterateRecursively may be set to recurse automatically into each entry as it is returned. This option affects the behaviour of the getNextObject method, which is defined in the OSIterator superclass. Other methods will override this behaviour. kIORegistryIterateParents may be set to iterate the parents of each entry, by default the children are iterated.

## Return Value

A created IORegistryIterator instance, to be released by the caller when it has finished with it.

## Overview

This method creates an IORegistryIterator that is set up with options to iterate children of the registry root entry, and to recurse automatically into entries as they are returned, or only when instructed. The iterator object keeps track of entries that have been recursed into previously to avoid loops.

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

iterateAll

Iterates all entries (with getNextObject) and returns a set of all returned entries.

iterateOver(IORegistryEntry *, const IORegistryPlane *, IOOptionBits)

Create an iterator rooted at a given registry entry.

reset

Exits all levels of recursion, restoring the iterator to its state at creation.

