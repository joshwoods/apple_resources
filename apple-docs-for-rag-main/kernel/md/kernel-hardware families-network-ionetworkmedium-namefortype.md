

- Kernel
- Hardware Families
- Network
- IONetworkMedium
-  nameForType 

# nameForType

Creates a name that describes a medium type.

``` source
static const OSSymbol * nameForType(
 IOMediumTypetype); 
```

## Parameters 

`type`  

A medium type. See IONetworkMedium.h for type encoding.

## Return Value

Returns an OSSymbol object is created based on the type provided.

## Overview

Given a medium type, creates an OSymbol object that describes the medium type. There is a 1-to-1 mapping between the medium type, and the medium name created by this method. The caller is responsible for releasing the OSSymbol object returned.

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

isEqualTo(const OSMetaClassBase *)

Tests for equality between a IONetworkMedium object and an OSObject.

medium

Factory method that allocates and initializes an IONetworkMedium object.

removeMedium

Removes an IONetworkMedium object from a dictionary.

serialize

Serializes the IONetworkMedium object.

