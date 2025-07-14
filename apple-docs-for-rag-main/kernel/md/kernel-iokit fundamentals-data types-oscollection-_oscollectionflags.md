

- Kernel
- IOKit Fundamentals
- Data Types
- OSCollection
-  \_OSCollectionFlags 

# \_OSCollectionFlags

``` source
typedef enum {
   kImmutable = 0x00000001,
   kSort = 0x00000002,
   kMASK = (
   unsigned) -1
} _OSCollectionFlags;
```

## Overview

Used with setOptions to indicate the collection's contents should or should not change.

An IORegistryEntry object marks collections immutable when set as properties of a registry entry that's attached to a plane. This is generally an advisory flag, used for debugging; setting it does not mean a collection will in fact disallow modifications.

## Topics

### Constants

kImmutable

