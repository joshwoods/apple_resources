

- Kernel
- IOKit Fundamentals
- Data Types
- OSCollectionIterator
-  isValid 

# isValid

Checks that the collection hasn't been modified during iteration.

``` source
virtual bool isValid(); 
```

## Return Value

`true` if the iterator is valid for continued use, `false` otherwise (typically because the iteration context has been modified).

## See Also

### Miscellaneous

free

Releases or deallocates any resources used by the OSCollectionIterator object.

getNextObject

Advances to and returns the next object in the iteration.

initWithCollection

Initializes an OSCollectionIterator for the provided collection object.

reset

Resets the iterator to the beginning of the collection, as if it had just been created.

withCollection

Creates and initializes an OSCollectionIterator for the provided collection object.

