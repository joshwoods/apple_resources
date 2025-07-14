

- Kernel
- IOKit Fundamentals
- Data Types
- OSSerialize
-  addXMLStartTag 

# addXMLStartTag

Appends an XML start tag to the XML stream.

``` source
virtual bool addXMLStartTag( 
 const OSMetaClassBase *object, 
 const char *tagString); 
```

## Parameters 

`object`  

The object being serialized.

`tagString`  

The name of the XML tag to emit; for example, "string".

## Return Value

`true` if an XML start tag for `tagString` is successfully added to the XML stream, `false` otherwise.

## Overview

This function emits the named tag, enclosed within a pair of angle brackets.

A class that implements serialization should call this function with the name of the XML tag that best represents the serialized contents of the object. A limited number of tags are supported by the user-space I/O Kit library:

- array

- dict

- integer

- key

- set

- string

A call to this function must be balanced with one to addXMLEndTag using the same `tagString`.

## See Also

### Miscellaneous

addChar

Appends a single character to the XML stream.

addString

Appends a C string to the XML stream.

addXMLEndTag

Appends an XML end tag to the XML stream.

clearText

Resets the OSSerialize object.

previouslySerialized

Checks whether the object has already been serialized into the XML stream, emitting a reference if it has.

text

Returns the XML text serialized so far.

withCapacity

Creates and initializes an empty OSSerialize object.

