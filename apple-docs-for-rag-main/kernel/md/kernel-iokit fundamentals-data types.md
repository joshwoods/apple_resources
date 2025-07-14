

- Kernel
- IOKit Fundamentals
-  Data Types 

API Collection

# Data Types

Create strings, numbers, collections, data objects, and the other standard types employed by drivers and kernel extensions.

## Topics

### Simple Types

OSBoolean

OSBoolean wraps a boolean value in a C++ object for use in Libkern collections.

OSString

OSString wraps a C string in a C++ object for use in Libkern collections.

OSNumber

OSNumber wraps an integer value in a C++ object for use in Libkern collections.

OSData

OSData wraps an array of bytes in a C++ object for use in Libkern collections.

### Collections

OSArray

OSArray provides an indexed store of objects.

OSDictionary

OSDictionary provides an associative store using strings for keys.

OSSet

OSSet provides an unordered set store of objects.

OSOrderedSet

OSOrderedSet provides an ordered set store of objects.

OSCollection

The abstract superclass for Libkern collections.

OSCollectionIterator

OSIterator

The abstract superclass for Libkern iterators.

### Signed Integers

LittleSInt16

LittleSInt32

LittleSInt64

BigSInt16

BigSInt32

BigSInt64

### Unsigned Integers

LittleUInt16

LittleUInt32

LittleUInt64

BigUInt16

BigUInt32

BigUInt64

U128

### Actions

OSAction

OSActionInterface

### Callback Methods

OSActionAbortedHandler

OSActionCancelHandler

OSDispatchMethod

OSKextRequestResourceCallback

Invoked to provide results for a kext resource request.

OSObjectApplierFunction

OSSerializerBlock

OSSerializerCallback

### Serialization

OSSerialize

OSSerialize coordinates serialization of Libkern C++ objects into an XML stream.

OSSerializer

### Base Types

OSSymbol

OSSymbol wraps a C string in a unique C++ object for use as keys in Libkern collections.

OSObject

OSObject is the concrete root class of the Libkern and I/O Kit C++ class hierarchy.

OSMetaClass

OSMetaClassBase

OSMetaClassBase is the abstract bootstrap class for the Libkern and I/O Kit run-time type information system.

OSObjectPtr

OSObjectRef

Additional Types

Find custom type definitions and pointer types for standard classes.

## See Also

### Resources

Memory

Allocate, map, free, and manage memory in the kernel.

Workflow and Control

Locks

