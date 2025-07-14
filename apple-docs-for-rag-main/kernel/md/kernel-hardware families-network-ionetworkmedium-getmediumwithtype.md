

- Kernel
- Hardware Families
- Network
- IONetworkMedium
-  getMediumWithType 

# getMediumWithType

Finds a medium object from a dictionary with a given type.

``` source
static IONetworkMedium * getMediumWithType(
 const OSDictionary *dict, 
 IOMediumType type, 
 IOMediumType mask = 0); 
```

## Parameters 

`dict`  

The dictionary to look for a matching entry.

`type`  

Search for an entry with this type.

`mask`  

The don't care bits in IOMediumType. Defaults to 0, which implies that a perfect match is desired.

## Return Value

Returns the first matching IONetworkMedium entry found, or 0 if no match was found.

## Overview

This method iterates through a dictionary and returns an IONetworkMedium entry with the given type. An optional mask supplies the don't care bits.

## See Also

### Miscellaneous

addMedium

Adds an IONetworkMedium object to a dictionary.

free

Frees the IONetworkMedium object.

getFlags

getIndex

getKey

getMediumWithIndex

Finds a medium object from a dictionary with a given index.

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

