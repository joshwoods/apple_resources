

- Kernel
- IOKit Fundamentals
- Data Types
- OSCollectionIterator
-  withCollection 

# withCollection

Creates and initializes an OSCollectionIterator for the provided collection object.

``` source
static OSCollectionIterator * withCollection(
 const OSCollection *inColl); 
```

## Parameters 

`inColl`  

The OSCollection-derived collection object to be iteratated.

## Return Value

A new instance of OSCollectionIterator, or `NULL` on failure.

## See Also

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

