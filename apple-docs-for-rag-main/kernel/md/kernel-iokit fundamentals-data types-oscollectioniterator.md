

- Kernel
- IOKit Fundamentals
- Data Types
-  OSCollectionIterator 

Class

# OSCollectionIterator

macOS 10.0+

``` source
class OSCollectionIterator : OSIterator
```

## Overview

OSCollectionIterator defines a consistent mechanism to iterate through the objects of an OSCollection. It expands on the basic interface of OSIterator to allow association of an iterator with a specific collection.

To use an OSCollectionIterator, you create it with the collection to be iterated, then call OSIterator as long as it returns an object:

\ OSCollectionIterator \* iterator = OSCollectionIterator::withCollection(myCollection); OSObject \* object; while (object = iterator-\>getNextObject()) { // do something with object } // optional if (!iterator-\>isValid()) { // report that collection changed during iteration } iterator-\>release(); \

Note that when iterating associative collections, the objects returned by `getNextObject` are keys; if you want to work with the associated values, simply look them up in the collection with the keys.

**Use Restrictions**

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are **unsafe** to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

OSCollectionIterator provides no concurrency protection.

## Topics

### Miscellaneous

free

Releases or deallocates any resources used by the OSCollectionIterator object.

getNextObject

Advances to and returns the next object in the iteration.

initWithCollection

Initializes an OSCollectionIterator for the provided collection object.

isValid

Checks that the collection hasn't been modified during iteration.

reset

Resets the iterator to the beginning of the collection, as if it had just been created.

withCollection

Creates and initializes an OSCollectionIterator for the provided collection object.

### Instance Methods

- free

- getMetaClass

- getNextObject

- initWithCollection

- isValid

- reset

### Type Methods

+ withCollection

## Relationships

### Inherits From

- OSIterator

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

OSIterator

The abstract superclass for Libkern iterators.

