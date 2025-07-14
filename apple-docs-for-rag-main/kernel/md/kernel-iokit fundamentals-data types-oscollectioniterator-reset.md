

- Kernel
- IOKit Fundamentals
- Data Types
- OSCollectionIterator
-  reset 

# reset

Resets the iterator to the beginning of the collection, as if it had just been created.

``` source
virtual void reset(); 
```

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

withCollection

Creates and initializes an OSCollectionIterator for the provided collection object.

