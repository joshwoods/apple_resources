

- Kernel
- IOKit Fundamentals
-  IORegistryIterator 

Class

# IORegistryIterator

An iterator over the registry.

macOS 10.0+

``` source
class IORegistryIterator : OSIterator
```

``` source
typedef struct IORegistryIterator IORegistryIterator;
```

## Overview

An iterator that can traverse the children or parents of a registry entry in a plane, and recurse. Access to the registry is protected against multiple threads, but an IORegistryIterator instance is for use by one thread only.

## Topics

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

iterateOver(const IORegistryPlane *, IOOptionBits)

Create an iterator rooted at the registry root.

iterateOver(IORegistryEntry *, const IORegistryPlane *, IOOptionBits)

Create an iterator rooted at a given registry entry.

reset

Exits all levels of recursion, restoring the iterator to its state at creation.

### Instance Methods

- enterEntry

- enterEntry

- exitEntry

- free

- getCurrentEntry

- getMetaClass

- getNextObject

- getNextObjectFlat

- getNextObjectRecursive

- isValid

- iterateAll

- reset

### Type Methods

+ iterateOver

+ iterateOver

## Relationships

### Inherits From

- OSIterator

## See Also

### Driver Registry

IORegistryEntry

The base class for all objects in the registry.

IOBSDNameMatching

Create a matching dictionary that specifies an IOService match based on BSD device name.

IOPrintPlane

Registry Utilities

Registry Keys

