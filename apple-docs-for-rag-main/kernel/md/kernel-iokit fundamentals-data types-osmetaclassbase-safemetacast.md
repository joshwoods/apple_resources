

- Kernel
- IOKit Fundamentals
- Data Types
- OSMetaClassBase
-  safeMetaCast 

# safeMetaCast

Casts an object is to the class managed by the given OSMetaClass.

``` source
static OSMetaClassBase * safeMetaCast( 
 const OSMetaClassBase *anObject, 
 const OSMetaClass *toMeta); 
```

## Parameters 

`anObject`  

A pointer to the object to be cast.

`toMeta`  

A pointer to a constant OSMetaClass for the desired target type.

## Return Value

`anObject` if the object is derived from the class managed by `toMeta`, otherwise `NULL`.

## Overview

It is far more convenient to use OSDynamicCast.

## See Also

### Miscellaneous

OSCheckTypeInst

Checks whether two objects are type-compatible.

OSDynamicCast

OSMemberFunctionCast

Converts a C++ member function pointer, relative to an instance, to a C-style pointer to function.

OSSafeRelease

Release an object if not `NULL`.

OSSafeReleaseNULL

OSTypeAlloc

OSTypeID

OSTypeIDInst

checkTypeInst

Checks whether an object instance is of the same class as another object instance (or a subclass of that class).

getMetaClass

Returns the OSMetaClass representing an OSMetaClassBase subclass.

getRetainCount

Abstract declaration of getRetainCount().

isEqualTo

Checks whether another object is equal to the receiver.

metaCast(const char *)

Casts this object is to the class managed by the named OSMetaClass.

metaCast(const OSMetaClass *)

Casts this object is to the class managed by the given OSMetaClass.

metaCast(const OSString *)

Casts this object is to the class managed by the named OSMetaClass.

metaCast(const OSSymbol *)

Casts this object is to the class managed by the named OSMetaClass.

release()

Abstract declaration of release.

release(int)

Abstract declaration of release(int freeWhen).

retain

Abstract declaration of retain().

serialize

Abstract declaration of serialize.

taggedRelease(const void *)

Abstract declaration of taggedRelease(const void \*).

taggedRelease(const void *, const int)

Abstract declaration of taggedRelease(const void \*, const int freeWhen).

taggedRetain

Abstract declaration of taggedRetain(const void \*).

