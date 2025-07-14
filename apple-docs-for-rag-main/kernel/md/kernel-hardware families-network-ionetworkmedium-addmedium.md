

- Kernel
- Hardware Families
- Network
- IONetworkMedium
-  addMedium 

# addMedium

Adds an IONetworkMedium object to a dictionary.

``` source
static bool addMedium(
 OSDictionary *dict, 
 const IONetworkMedium *medium); 
```

## Parameters 

`dict`  

An OSDictionary object where the medium object should be added as a new entry.

`medium`  

The IONetworkMedium object to add to the dictionary.

## Return Value

Returns true on success, false otherwise.

## Overview

A helper function to add an IONetworkMedium object to a given dictionary. The name of the medium is used as the key for the new dictionary entry.

## See Also

### Miscellaneous

free

Frees the IONetworkMedium object.

getFlags

getIndex

getKey

getMediumWithIndex

Finds a medium object from a dictionary with a given index.

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

