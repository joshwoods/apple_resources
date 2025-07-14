

- DriverKit
-  OSSet 

Class

# OSSet

OSSet provides an unordered set store of objects.

DriverKitiOSiPadOSmacOS

``` source
class OSSet;
```

## Overview

OSSet is a container for Libkern C++ objects (those derived from OSMetaClassBase, in particular OSObject). Storage and access follow basic set logic: you can add or remove an object, and test whether the set contains a particular object. A given object is only stored in the set once, and there is no ordering of objects in the set. A subclass OSOrderedSet, provides for ordered set logic.

As with all Libkern collection classes, OSSet retains objects added to it, and releases objects removed from it. An OSSet also grows as necessary to accommodate new objects, unlike Core Foundation collections (it does not, however, shrink).

## Use Restrictions

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are unsafe to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

OSSet provides no concurrency protection; it’s up to the usage context to provide any protection necessary. Some portions of the I/O Kit, such as `IORegistryEntry`, handle synchronization via defined member functions for setting properties.

## Topics

### Instance Methods

containsObject

getAnyObject

Returns an arbitrary (not random) object from the set.

init

member

Checks the set for the presence of an object.

merge

Adds the contents of an OSet to the set.

removeObject

setObject

Adds an object to the OSSet if it is not already present.

### Type Methods

withArray

Creates and initializes an OSSet populated with the contents of an OSArray.

withCapacity

withObjects

Creates and initializes an OSSet populated with objects provided.

## Relationships

### Inherits From

- OSArray

### Inherited By

- OSOrderedSet

## See Also

### Data Types

IOCallOnceBlock

IOCallOnceFlag

IOCommand

IOCommandPool

IOCommandPoolPtr

IOCommandPtr

IODMACommand

An object that converts memory references to I/O bus addresses.

IODMACommandSpecification

IODispatchAction

IOHistogramReporter_IVars

IOReportLegendEntry

IOReporter_IVars

IOSimpleReporter_IVars

IOStateReporter_IVars

IOStateReporter_valueSelector

