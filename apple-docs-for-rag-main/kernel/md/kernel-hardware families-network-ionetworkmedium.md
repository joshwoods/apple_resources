

- Kernel
- Hardware Families
- Network
-  IONetworkMedium 

Class

# IONetworkMedium

An object that encapsulates information about a network medium (i.e. 10Base-T, or 100Base-T Full Duplex).

macOS 10.6+

``` source
class IONetworkMedium : OSObject
```

## Overview

The main purpose of this object is for a network driver to advertise its media capability, through a collection of IONetworkMedium objects stored in a dictionary in its property table. IONetworkMedium supports serialization, and will encode its properties in the form of a dictionary to the serialization stream when instructed. This will allow a user-space application to browse the set of media types supported by the controller.

## Topics

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

nameForType

Creates a name that describes a medium type.

removeMedium

Removes an IONetworkMedium object from a dictionary.

serialize

Serializes the IONetworkMedium object.

### Instance Variables

_reserved

### Instance Methods

- getKey

- free

- getFlags

- getIndex

- getMetaClass

- getName

- getSpeed

- getType

- init

- isEqualTo

- isEqualTo

- serialize

### Type Methods

+ addMedium

+ getMediumWithIndex

+ getMediumWithType

+ medium

+ nameForType

+ removeMedium

## Relationships

### Inherits From

- OSObject

## See Also

### Network Data

IONetworkData

An object that manages a fixed-size named buffer.

IOPacketQueue

Implements a bounded FIFO queue of mbuf packets.

IOPacketBufferConstraints

