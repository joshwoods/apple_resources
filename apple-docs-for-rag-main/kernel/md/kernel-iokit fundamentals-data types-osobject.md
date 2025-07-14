

- Kernel
- IOKit Fundamentals
- Data Types
-  OSObject 

Class

# OSObject

OSObject is the concrete root class of the Libkern and I/O Kit C++ class hierarchy.

macOS 10.0+

``` source
class OSObject : OSMetaClassBase
```

## Overview

OSObject defines the minimal functionality required of Libkern and I/O Kit C++ classes: tie-in to the run-time type information facility, the dynamic allocation/initialization paradigm, and reference counting. While kernel extensions are free to use their own C++ classes internally, any interaction they have with Libkern or the I/O Kit will require classes ultimately derived from OSObject.

**Run-Time Type Information**

OSObject is derived from the abstract root class OSMetaClassBase, which declares (and defines many of) the primitives on which the run-time type information facility is based. A parallel inheritance hierarchy of metaclass objects provides run-time introspection, including access to class names, inheritance, and safe type-casting. See OSMetaClass for more information.

**Dynamic Allocation/Initialization**

The kernel-resident C++ runtime does not support exceptions, so Libkern classes cannot use standard C++ object constructors and destructors, which use exceptions to report errors. To support error-handling during instance creation, then, OSObject separates object allocation from initialization. You can create a new OSObject-derived instance with the `new` operator, but this does nothing more than allocate memory and initialize the reference count to 1. Following this, you must call a designated initialization function and check its `bool` return value. If the initialization fails, you must immediately call release on the instance and handle the failure in whatever way is appropriate. Many Libkern and I/O Kit classes define static instance-creation functions (beginning with the word "with") to make construction a one-step process for clients.

**Reference Counting**

OSObject provides reference counting services using the retain, release(), release(int freeWhen) and free functions. The public interface to the reference counting is retain, and release; release(int freeWhen) is provided for objects that have internal retain cycles.

In general, a subclass is expected to only override free. It may also choose to override release(int freeWhen) if the object has a circular retain count, as noted above.

**Use Restrictions**

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are **unsafe** to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

**Concurrency Protection**

The basic features of OSObject are thread-safe. Most Libkern subclasses are not, and require locking or other protection if instances are shared between threads. I/O Kit driver objects are either designed for use within thread-safe contexts or designed to inherently be thread-safe. Always check the individual class documentation to see what steps are necessary for concurrent use of instances.

## Topics

### Miscellaneous

free

Deallocates/releases resources held by the object.

getRetainCount

Returns the reference count of the object.

init

Initializes a newly-allocated object.

operator delete

Frees the memory of the object itself.

operator new

Allocates memory for an instance of the class.

release()

Releases a reference to the object, freeing it immediately if the reference count drops to zero.

release(int)

Releases a reference to an object, freeing it immediately if the reference count drops below the specified threshold.

retain

Retains a reference to the object.

serialize

Overridden by subclasses to archive the receiver into the provided OSSerialize object.

taggedRelease(const void *)

Releases a tagged reference to an object, freeing it immediately if the reference count drops to zero.

taggedRelease(const void *, const int)

Releases a tagged reference to an object, freeing it immediately if the reference count drops below the specified threshold.

taggedRetain

Retains a reference to the object with an optional tag used for reference-tracking.

### Instance Methods

- CopyDispatchQueue

- Dispatch

- SetDispatchQueue

- free

- getMetaClass

- getRetainCount

- init

- release

- release

Releases the OSObject instance

- retain

Retains the OSObject instance

- serialize

- taggedRelease

- taggedRelease

- taggedRetain

### Type Methods

+ CopyDispatchQueue_Invoke

+ SetDispatchQueue_Invoke

## Relationships

### Inherits From

- OSMetaClassBase

## See Also

### Base Types

OSSymbol

OSSymbol wraps a C string in a unique C++ object for use as keys in Libkern collections.

OSMetaClass

OSMetaClassBase

OSMetaClassBase is the abstract bootstrap class for the Libkern and I/O Kit run-time type information system.

OSObjectPtr

OSObjectRef

Additional Types

Find custom type definitions and pointer types for standard classes.

