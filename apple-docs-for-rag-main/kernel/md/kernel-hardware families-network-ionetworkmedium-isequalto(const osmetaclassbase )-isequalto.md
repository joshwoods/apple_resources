

- Kernel
- Hardware Families
- Network
- IONetworkMedium
-  isEqualTo(const OSMetaClassBase \*) 

# isEqualTo(const OSMetaClassBase \*)

Tests for equality between a IONetworkMedium object and an OSObject.

``` source
virtual bool isEqualTo(
 const OSMetaClassBase *obj) const; 
```

## Parameters 

`obj`  

An OSObject to test against an IONetworkMedium object.

## Return Value

Returns true if equal, false otherwise.

## Overview

The OSObject is considered equal to the IONetworkMedium object if the OSObject is an IONetworkMedium, and they have similar properties assigned to them during initialization.

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

isEqualTo(const IONetworkMedium *)

Tests for equality between two IONetworkMedium objects.

medium

Factory method that allocates and initializes an IONetworkMedium object.

nameForType

Creates a name that describes a medium type.

removeMedium

Removes an IONetworkMedium object from a dictionary.

serialize

Serializes the IONetworkMedium object.

