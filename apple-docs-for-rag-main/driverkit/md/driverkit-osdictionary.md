

- DriverKit
-  OSDictionary 

Class

# OSDictionary

A container for a collection with elements that are key-value pairs.

DriverKitiOSiPadOSmacOS

``` source
class OSDictionary;
```

## Overview

OSDictionary is a collection class for objects derived from OSObject. Storage and access are associative, based on keys that are uniqued OSObjects. OSString is commonly used as a key since it is uniqued. When adding an object to an OSDictionary, you provide a string identifier, which can then used to retrieve that object or remove it from the dictionary. Setting an object with a key that already has an associated object replaces the original object.

You must generally cast retrieved objects from OSObject to the desired class using the OSDynamicCast macro. This macro returns the object cast to the desired class, or `NULL` if the object isn’t derived from that class.

As with all DriverKit collection classes, OSDictionary retains objects added to it, and releases objects removed from it (or replaced). An OSDictionary also grows as necessary to accommodate new objects.

OSArray provides no concurrency protection; it’s up to the usage context to provide any protection necessary.

## Topics

### Creating a Dictionary

withCapacity

Allocates an OSDictionary object with preallocated capacity.

withDictionary

Allocates an OSDictionary object with given members and preallocated capacity.

withObjects

Allocates an OSDictionary object with given members and preallocated capacity.

OSDictionaryCreate

merge

Adds all members of a dictionary to this dictionary.

free

flushCollection

Removes and drops references to all members of dictionary.

### Accessing Keys and Values

getObject

Returns a member of the dictionary.

getObject

Returns a member of the dictionary.

setObject

Add or replace an object in the dictionary.

setObject

Add or replace an object in the dictionary.

removeObject

Remove an object by key from the dictionary.

removeObject

Remove an object by key from the dictionary.

iterateObjects

Iterates the dictionary calling a callback block for each member.

iterateObjects

Iterates the dictionary calling a callback block for each member.

OSDictionaryIterateObjectsBlock

OSDictionaryIterateObjectsCallback

### Getting and Setting Values

OSDictionaryGetValue

OSDictionaryGetStringValue

OSDictionaryGetUInt64Value

OSDictionarySetValue

OSDictionarySetStringValue

OSDictionarySetUInt64Value

OSDictionaryPtr

### Inspecting a Dictionary

ensureCapacity

Allocates capacity for members in dictionary.

getCapacity

Returns count of currently allocated capacity for members in dictionary.

getCount

Returns count of members in dictionary.

OSDictionaryGetCount

### Modifying the Dictionary Items

OSDictionaryApply

OSDictionaryApplier

### Comparing Dictionaries

isEqualTo

Compares all members of two dictionaries with isEqualTo().

isEqualTo

Compares certain members of two dictionaries with isEqualTo().

isEqualTo

Compares the dictionary with an OSObject

## Relationships

### Inherits From

- OSCollection

## See Also

### Registry data types

OSArray

A container for an ordered, random-access collection of objects.

OSBoolean

A container for a true or false value.

OSData

A container for untyped data.

OSNumber

A container for an integer value.

OSString

A container for managing an array of characters.

OSSerialization

A container for one or more objects, serialized in a binary data format that is suitable for messaging.

OSCollection

The base class for DriverKit collection objects.

OSContainer

The base class for DriverKit data objects.

OSObject

The base class for DriverKit objects

OSSymbol

A container for managing an array of characters.

IOFixed

A fixed-point number.

