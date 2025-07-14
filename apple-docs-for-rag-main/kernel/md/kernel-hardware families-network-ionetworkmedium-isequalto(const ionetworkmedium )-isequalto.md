

- Kernel
- Hardware Families
- Network
- IONetworkMedium
-  isEqualTo(const IONetworkMedium \*) 

# isEqualTo(const IONetworkMedium \*)

Tests for equality between two IONetworkMedium objects.

``` source
virtual bool isEqualTo(
 const IONetworkMedium *medium) const; 
```

## Parameters 

`medium`  

An IONetworkMedium to test against the IONetworkMedium object being called.

## Return Value

Returns true if equal, false otherwise.

## Overview

Two IONetworkMedium objects are considered equal if they have similar properties assigned to them during initialization.

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

getMediumWithType

Finds a medium object from a dictionary with a given type.

getName

getSpeed

getType

init

Initializes an IONetworkMedium object.

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

