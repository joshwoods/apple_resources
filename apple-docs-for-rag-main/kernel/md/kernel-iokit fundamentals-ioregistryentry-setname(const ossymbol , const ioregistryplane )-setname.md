

- Kernel
- IOKit Fundamentals
- IORegistryEntry
-  setName(const OSSymbol \*, const IORegistryPlane \*) 

# setName(const OSSymbol \*, const IORegistryPlane \*)

Sets a name for the registry entry, in a particular plane, or globally.

``` source
virtual void setName(
 const OSSymbol *name, 
 const IORegistryPlane *plane = 0 ); 
```

## Parameters 

`name`  

An OSSymbol which will be retained.

`plane`  

The plane object, or zero to set the global name.

## Overview

Entries can be named in a particular plane, or globally. If the plane is specified the name applies only to that plane, otherwise the global name is set. The global name defaults to the entry's meta class name if it has not been named.

## See Also

### Miscellaneous

attachToChild

Method called in the parent entry when a child attaches.

attachToParent

Attaches a entry to a parent entry in a plane.

childFromPath

Looks up a registry entry by relative path.

compareName

Compares the name of the entry with one name, and optionally returns the matching name.

compareNames

Compares the name of the entry with one or more names, and optionally returns the matching name.

copyChildEntry

Returns an registry entry's first child entry in a plane. Available in macOS 10.1 or later.

copyLocation

Returns the location string assigned to the registry entry as an OSSymbol.

copyName

Returns the name assigned to the registry entry as an OSSymbol.

copyParentEntry

Returns an registry entry's first parent entry in a plane. Available in macOS 10.1 or later.

copyProperty(const char *)

Synchronized method to obtain a property from a registry entry's property table.

copyProperty(const char *, const IORegistryPlane *, IOOptionBits)

Synchronized method to obtain a property from a registry entry or one of its parents (or children) in the hierarchy. Available in macOS 10.1 or later.

copyProperty(const OSString *)

Synchronized method to obtain a property from a registry entry's property table.

copyProperty(const OSString *, const IORegistryPlane *, IOOptionBits)

Synchronized method to obtain a property from a registry entry or one of its parents (or children) in the hierarchy. Available in macOS 10.1 or later.

copyProperty(const OSSymbol *)

Synchronized method to obtain a property from a registry entry's property table.

copyProperty(const OSSymbol *, const IORegistryPlane *, IOOptionBits)

Synchronized method to obtain a property from a registry entry or one of its parents (or children) in the hierarchy. Available in macOS 10.1 or later.

dealiasPath

Strips any aliases from the head of path and returns the full path.

detachAbove

Detaches an entry from all its parent entries in a plane.

detachAll

Detaches an entry and all its children recursively in a plane.

detachFromChild

Detaches a child entry from its parent in a plane.

detachFromParent

Detaches an entry from a parent entry in a plane.

dictionaryWithProperties

Synchronized method to obtain copy a registry entry's property table.

free

Standard free method for all IORegistryEntry subclasses.

fromPath(const char *, const IORegistryPlane *, char *, int *)

Looks up a registry entry by relative path.

fromPath(const char *, const IORegistryPlane *, char *, int *, IORegistryEntry *)

Looks up a registry entry by path.

getChildEntry

Returns an registry entry's first child entry in a plane.

getChildIterator

Returns an iterator over an registry entry's child entries in a plane.

getDepth

Counts the maximum number of entries between an entry and the registry root, in a plane.

getGenerationCount

Returns an generation count for all registry changing operations.

getLocation

Returns the location string assigned to the registry entry as a C-string.

getName

Returns the name assigned to the registry entry as a C-string.

getParentEntry

Returns an registry entry's first parent entry in a plane.

getParentIterator

Returns an iterator over an registry entry's parent entries in a specified plane.

getPath

Create a path for a registry entry.

getPathComponent

Create a path component for a registry entry.

getPlane

Looks up the plane object by a C-string name.

getProperty(const char *)

Synchronized method to obtain a property from a registry entry's property table.

getProperty(const char *, const IORegistryPlane *, IOOptionBits)

Synchronized method to obtain a property from a registry entry or one of its parents (or children) in the hierarchy.

getProperty(const OSString *)

Synchronized method to obtain a property from a registry entry's property table.

getProperty(const OSString *, const IORegistryPlane *, IOOptionBits)

Synchronized method to obtain a property from a registry entry or one of its parents (or children) in the hierarchy.

getProperty(const OSSymbol *)

Synchronized method to obtain a property from a registry entry's property table.

getProperty(const OSSymbol *, const IORegistryPlane *, IOOptionBits)

Synchronized method to obtain a property from a registry entry or one of its parents (or children) in the hierarchy.

getPropertyTable

Unsynchronized accessor to a registry entry's property table.

getRegistryEntryID

Returns an ID for the registry entry that is global to all tasks.

getRegistryRoot

Returns a pointer to the root instance of the registry.

init

Standard init method for all IORegistryEntry subclasses.

inPlane

Determines whether a registry entry is attached in a plane.

isChild

Determines whether a registry entry is the child of another in a plane.

isParent

Determines whether a registry entry is the parent of another in a plane.

makePlane

Constructs an IORegistryPlane object.

removeProperty

Synchronized method to remove a property from a registry entry's property table.

removeProperty(const OSString *)

Synchronized method to remove a property from a registry entry's property table.

removeProperty(const OSSymbol *)

Synchronized method to remove a property from a registry entry's property table.

runPropertyAction

Single thread a call to an action w.r.t. the property lock

serializeProperties

Synchronized method to serialize a registry entry's property table.

setLocation

Sets a location string for the registry entry, in a particular plane, or globally.

setName(const char *, const IORegistryPlane *)

Sets a name for the registry entry, in a particular plane, or globally.

setProperties

Optionally supported external method to set properties in a registry entry.

setProperty

Synchronized method to construct and add an OSData property to a registry entry's property table.

setProperty(const char *, bool)

Synchronized method to construct and add an OSBoolean property to a registry entry's property table.

setProperty(const char *, const char *)

Synchronized method to construct and add a OSString property to a registry entry's property table.

setProperty(const char *, OSObject *)

Synchronized method to add a property to a registry entry's property table.

setProperty(const char *, unsigned long long, unsigned int)

Synchronized method to construct and add an OSNumber property to a registry entry's property table.

setProperty(const OSString *, OSObject *)

Synchronized method to add a property to a registry entry's property table.

setProperty(const OSSymbol *, OSObject *)

Synchronized method to add a property to a registry entry's property table.

setPropertyTable

Replace a registry entry's property table.

