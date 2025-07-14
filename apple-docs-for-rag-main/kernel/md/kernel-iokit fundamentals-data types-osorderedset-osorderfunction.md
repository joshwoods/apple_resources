

- Kernel
- IOKit Fundamentals
- Data Types
- OSOrderedSet
-  OSOrderFunction 

# OSOrderFunction

The sorting function used by an OSOrderedSet to order objects.

``` source
typedef SInt32 ( *OSOrderFunction)(
   const OSMetaClassBase *obj1,
   const OSMetaClassBase *obj2,
   void *context);
```

## Parameters 

`obj1`  

An object from the ordered set. May be `NULL`.

`obj2`  

The object being ordered within the ordered set. May be `NULL`.

`context`  

A pointer to a user-provided context. May be `NULL`.

## Return Value

A comparison result of the object:

- a negative value if obj2 should precede obj1,

- a positive value if obj1 should precede obj2,

- and 0 if obj1 and obj2 have an equivalent ordering.

