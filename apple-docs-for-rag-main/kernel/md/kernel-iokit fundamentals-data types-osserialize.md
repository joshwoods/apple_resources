

- Kernel
- IOKit Fundamentals
- Data Types
-  OSSerialize 

Class

# OSSerialize

OSSerialize coordinates serialization of Libkern C++ objects into an XML stream.

macOS 10.0+

``` source
class OSSerialize : OSObject
```

## Overview

This class is for the most part internal to the OSContainer classes, used for transferring property tables between the kernel and user space. It should not be used directly. Classes that participate in serialization override the OSObject::serialize . function.

**Use Restrictions**

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are **unsafe** to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

OSSerialize provides no concurrency protection; it's up to the usage context to provide any protection necessary. Some portions of the I/O Kit, such as IORegistryEntry, handle synchronization via defined member functions for serializing properties.

## Topics

### Miscellaneous

addChar

Appends a single character to the XML stream.

addString

Appends a C string to the XML stream.

addXMLEndTag

Appends an XML end tag to the XML stream.

addXMLStartTag

Appends an XML start tag to the XML stream.

clearText

Resets the OSSerialize object.

previouslySerialized

Checks whether the object has already been serialized into the XML stream, emitting a reference if it has.

text

Returns the XML text serialized so far.

withCapacity

Creates and initializes an empty OSSerialize object.

### Instance Methods

- addBinary

- addBinaryObject

- addChar

- addString

- addXMLEndTag

- addXMLStartTag

- binarySerialize

- binarySerializeInternal

- clearText

- endBinaryCollection

- ensureCapacity

- free

- getCapacity

- getCapacityIncrement

- getLength

- getMetaClass

- initWithCapacity

- previouslySerialized

- setCapacityIncrement

- setIndexed

- text

### Type Methods

+ binaryWithCapacity

+ withCapacity

## Relationships

### Inherits From

- OSObject

## See Also

### Serialization

OSSerializer

