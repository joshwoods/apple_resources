

- DriverKit
-  OSOrderedSet 

Class

# OSOrderedSet

OSOrderedSet provides an ordered set store of objects.

DriverKitiOSiPadOSmacOS

``` source
class OSOrderedSet;
```

## Overview

OSOrderedSet is a container for Libkern C++ objects (those derived from OSMetaClassBase, in particular OSObject). Storage and access follow ordered set logic. A given object is stored in the set only once, but you can:

- Define a sorting function for automated ordering (upon addition only)

- Manually insert new objects in the set (overriding sorting)

- Add and remove objects in the set

- Test whether the set contains a particular object

- Get the object stored at a particular index.

Note that automated ordering is performed only upon addition of objects and depends on the existing objects being properly sorted. There is no function to re-sort the contents of an OSOrderedSet or to change the ordering function. In general, you should either use the one ordered-insertion function, or the indexed-insertion functions, and not mix the two.

As with all Libkern collection classes, OSOrderedSet retains objects added to it, and releases objects removed from it. An OSOrderedSet also grows as necessary to accommodate new objects, unlike Core Foundation collections (it does not, however, shrink).

## Use Restrictions

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are unsafe to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

OSOrderedSet provides no concurrency protection; it’s up to the usage context to provide any protection necessary. Some portions of the I/O Kit, such as `IORegistryEntry`, handle synchronization via defined member functions for setting properties.

## Topics

### Instance Methods

free

getFirstObject

The object at index 0 in the ordered set if there is one, otherwise `NULL`.

getLastObject

The last object in the ordered set if there is one, otherwise `NULL`.

init

orderObject

Calls the ordered set’s order function against a `NULL` object.

setFirstObject

Adds an object to the OSOrderedSet at index 0 if it is not already present.

setLastObject

Adds an object at the end of the OSOrderedSet if it is not already present.

setObject

Adds an object to the OSOrderedSet if it is not already present, storing it in sorted order if there is an order function.

### Type Methods

withCapacity

## Relationships

### Inherits From

- OSSet

## See Also

### Data Types

IOCallOnceBlock

IOCallOnceFlag

IOCommand

IOCommandPool

IOCommandPoolPtr

IOCommandPtr

IODMACommand

An object that converts memory references to I/O bus addresses.

IODMACommandSpecification

IODispatchAction

IOHistogramReporter_IVars

IOReportLegendEntry

IOReporter_IVars

IOSimpleReporter_IVars

IOStateReporter_IVars

IOStateReporter_valueSelector

