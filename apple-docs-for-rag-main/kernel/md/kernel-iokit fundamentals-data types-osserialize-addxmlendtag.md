

- Kernel
- IOKit Fundamentals
- Data Types
- OSSerialize
-  addXMLEndTag 

# addXMLEndTag

Appends an XML end tag to the XML stream.

``` source
virtual bool addXMLEndTag(
 const char *tagString); 
```

## Parameters 

`tagString`  

The name of the XML tag to emit; for example, "string".

## Return Value

`true` if an XML end tag for `tagString` is successfully added to the XML stream, `false` otherwise.

## Overview

This function emits the named tag, preceded by a slash character to indicate the closing of an entity, all enclosed within a pair of angle brackets.

A call to this function must balance an earlier call to addXMLStartTag using the same `tagString`.

## See Also

### Miscellaneous

addChar

Appends a single character to the XML stream.

addString

Appends a C string to the XML stream.

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

