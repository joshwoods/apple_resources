

- Kernel
- IOKit Fundamentals
- Data Types
-  OSMetaClass 

Class

# OSMetaClass

macOS 10.0+

``` source
class OSMetaClass : OSMetaClassBase
```

## Topics

### Instance Methods

- alloc

- checkMetaCast

- getClassName

- getClassNameSymbol

- getClassSize

- getInstanceCount

- getKmodName

- getMetaClass

- getRetainCount

- getSuperClass

- instanceConstructed

- instanceDestructed

- release

- release

- reservedCalled

- retain

- serialize

- taggedRelease

- taggedRelease

- taggedRetain

### Type Methods

+ allocClassWithName

+ allocClassWithName

+ allocClassWithName

+ checkMetaCastWithName

+ checkMetaCastWithName

+ checkMetaCastWithName

+ checkModLoad

+ considerUnloads

+ getClassDictionary

+ getMetaClassWithName

+ logError

+ modHasInstance

+ postModLoad

+ preModLoad

+ printInstanceCounts

+ reportModInstances

+ serializeClassDictionary

## Relationships

### Inherits From

- OSMetaClassBase

## See Also

### Base Types

OSSymbol

OSSymbol wraps a C string in a unique C++ object for use as keys in Libkern collections.

OSObject

OSObject is the concrete root class of the Libkern and I/O Kit C++ class hierarchy.

OSMetaClassBase

OSMetaClassBase is the abstract bootstrap class for the Libkern and I/O Kit run-time type information system.

OSObjectPtr

OSObjectRef

Additional Types

Find custom type definitions and pointer types for standard classes.

