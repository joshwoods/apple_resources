

- Kernel
- IOKit Fundamentals
- Data Types
-  OSIterator 

Class

# OSIterator

The abstract superclass for Libkern iterators.

macOS 10.0+

``` source
class OSIterator : OSObject
```

## Overview

OSIterator is the abstract superclass for all Libkern C++ object iterators. It defines the basic interface for iterating and resetting. See OSCollection and OSCollectionIterator for more information.

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are **unsafe** to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

OSIterator provides no concurrency protection.

## Topics

### Miscellaneous

getNextObject

Advances to and returns the next object in the iteration.

isValid

Check that the collection hasn't been modified during iteration.

reset

Resets the iterator to the beginning of the collection, as if it had just been created.

### Instance Methods

- getMetaClass

- getNextObject

- isValid

- reset

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

OSCollection

The abstract superclass for Libkern collections.

OSCollectionIterator

