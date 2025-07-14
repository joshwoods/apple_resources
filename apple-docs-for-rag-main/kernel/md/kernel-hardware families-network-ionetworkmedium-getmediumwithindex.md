

- Kernel
- Hardware Families
- Network
- IONetworkMedium
-  getMediumWithIndex 

# getMediumWithIndex

Finds a medium object from a dictionary with a given index.

``` source
static IONetworkMedium * getMediumWithIndex(
 const OSDictionary *dict, 
 UInt32 index, 
 UInt32 mask = 0); 
```

## Parameters 

`dict`  

The dictionary to look for a matching entry.

`index`  

Search for an entry with the given index.

`mask`  

The don't care bits in index. Defaults to 0, which implies that a perfect match is desired.

## Return Value

Returns the first matching IONetworkMedium entry found, or 0 if no match was found.

## Overview

This method iterates through a dictionary and returns an IONetworkMedium entry with the given index. An optional mask supplies the don't care bits.

## See Also

### Miscellaneous

addMedium

Adds an IONetworkMedium object to a dictionary.

free

Frees the IONetworkMedium object.

getFlags

getIndex

getKey

getMediumWithType

Finds a medium object from a dictionary with a given type.

getName

getSpeed

getType

init

Initializes an IONetworkMedium object.

isEqualTo(const IONetworkMedium *)

Tests for equality between two IONetworkMedium objects.

isEqualTo(const OSMetaClassBase *)

Tests for equality between a IONetworkMedium object and an OSObject.

medium

Factory method that allocates and initializes an IONetworkMedium object.

nameForType

Creates a name that describes a medium type.

removeMedium

Removes an IONetworkMedium object from a dictionary.

serialize

Serializes the IONetworkMedium object.

