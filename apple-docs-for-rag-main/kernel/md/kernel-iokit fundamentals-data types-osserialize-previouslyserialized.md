

- Kernel
- IOKit Fundamentals
- Data Types
- OSSerialize
-  previouslySerialized 

# previouslySerialized

Checks whether the object has already been serialized into the XML stream, emitting a reference if it has.

``` source
virtual bool previouslySerialized(
 const OSMetaClassBase *object); 
```

## Parameters 

`object`  

The object to check.

## Return Value

`true` if `object` has already been serialized by this OSSerialize object and a reference to it is successfully added to the XML stream, `false` otherwise.

## Overview

This function both reduces the size of generated XML by emitting shorter references to existing objects with the same value (particularly for OSString, OSSymbol, and OSData), and also preserves instance references so that the user-space I/O Kit library can reconstruct an identical graph of object relationships.

All classes that override OSObject::serialize. should call this function before doing any actual serialization; if it returns `true`, the `serialize` implementation can immediately return `true`.

## See Also

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

text

Returns the XML text serialized so far.

withCapacity

Creates and initializes an empty OSSerialize object.

