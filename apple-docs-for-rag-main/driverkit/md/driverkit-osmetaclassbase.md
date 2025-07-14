

- DriverKit
-  OSMetaClassBase 

Class

# OSMetaClassBase

Base class for DriverKit objects.

DriverKitiOSiPadOSmacOS

``` source
class OSMetaClassBase;
```

## Topics

### Managing the Object Lifecycle

retain

Retains the OSObject instance

release

Releases the OSObject instance

### Casting to Different Types

requiredMetaCast

Internal helper for OSRequiredCast. Not to be called directly.

safeMetaCast

Internal helper for OSDynamicCast. Not to be called directly.

### Getting Meta Information

IsRemote

GetClass

Internal helper for GetClassName. Not to be called directly.

GetClassName

Returns the name of the class given an OSObject pointer.

getMetaClass

Internal helper for GetClassName. Not to be called directly.

### Comparing Objects

isEqualTo

Compares two objects

### Managing Runtime Internals

Invoke

Runtime internals

Dispatch

Runtime internals

### Instance Methods

GetClassName

getRetainCount

operator new

### Instance Properties

meta

refcount

reserved

## Relationships

### Inherited By

- OSMetaClass
- OSObject

## See Also

### Base Classes

OSMetaClass

Base class for DriverKit runtime class system. Not called directly.

