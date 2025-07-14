

- Kernel
- IOKit Fundamentals
- Data Types
- OSMetaClassBase
-  isEqualTo 

# isEqualTo

Checks whether another object is equal to the receiver.

``` source
virtual bool isEqualTo(
 const OSMetaClassBase *anObject) const; 
```

## Parameters 

`anObject`  

The object to copmare to the receiver.

## Return Value

`true` if the objects are equal, `false` otherwise.

## Overview

OSMetaClassBase implements this as a direct pointer comparison, since it has no other information to judge equality by. Subclasses generally override this function to do a more meaningful comparison. For example, OSString implements it to return `true` if `anObject` is derived from OSString and represents the same C string.

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

safeMetaCast

Casts an object is to the class managed by the given OSMetaClass.

serialize

Abstract declaration of serialize.

taggedRelease(const void *)

Abstract declaration of taggedRelease(const void \*).

taggedRelease(const void *, const int)

Abstract declaration of taggedRelease(const void \*, const int freeWhen).

taggedRetain

Abstract declaration of taggedRetain(const void \*).

