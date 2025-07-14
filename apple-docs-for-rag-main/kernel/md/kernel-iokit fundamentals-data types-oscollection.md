

- Kernel
- IOKit Fundamentals
- Data Types
-  OSCollection 

Class

# OSCollection

The abstract superclass for Libkern collections.

macOS 10.0+

``` source
class OSCollection : OSObject
```

## Overview

OSCollection is the abstract superclass for all Libkern C++ object collections. It defines the necessary interfaces for managing storage space and iterating through an arbitrary collection (see the OSIterator and OSCollectionIterator classes). It is up to concrete subclasses to define their specific content management functions.

**Use Restrictions**

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are **unsafe** to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

OSCollection provides no concurrency protection; it's up to the usage context to provide any protection necessary. Some portions of the I/O Kit, such as IORegistryEntry, handle synchronization via defined member functions for setting properties.

## Topics

### Miscellaneous

copyCollection

Creates a deep copy of a collection.

ensureCapacity

Ensures the collection has enough space to store the requested number of objects.

flushCollection

Empties the collection, releasing any objects retained.

getCapacity

Returns the number of objects the collection can store without reallocating.

getCapacityIncrement

Returns the storage increment of the collection.

getCount

Returns the number of objects in the collection.

getNextObjectForIterator

Returns the next member of a collection.

haveUpdated

Tracks updates to the collection.

init

Initializes the OSCollection object.

initIterator

Initializes the iteration context for a collection subclass.

iteratorSize

Returns the size in bytes of a subclass's iteration context.

setCapacityIncrement

Sets the storage increment of the collection.

### DataTypes

_OSCollectionFlags

### Instance Methods

- copyCollection

- ensureCapacity

- flushCollection

- getCapacity

- getCapacityIncrement

- getCount

- getMetaClass

- getNextObjectForIterator

- haveUpdated

- init

- initIterator

- iterateObjects

- iterateObjects

- iteratorSize

- setCapacityIncrement

- setOptions

Recursively sets option bits in this collection and all child collections.

## Relationships

### Inherits From

- OSObject

## See Also

### Collections

OSArray

OSArray provides an indexed store of objects.

OSDictionary

OSDictionary provides an associative store using strings for keys.

OSSet

OSSet provides an unordered set store of objects.

OSOrderedSet

OSOrderedSet provides an ordered set store of objects.

OSCollectionIterator

OSIterator

The abstract superclass for Libkern iterators.

