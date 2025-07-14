

- Kernel
- IOKit Fundamentals
- Data Types
- OSSerialize
-  withCapacity 

# withCapacity

Creates and initializes an empty OSSerialize object.

``` source
static OSSerialize * withCapacity(
 unsigned intcapacity); 
```

## Parameters 

`capacity`  

The initial size of the XML buffer.

## Return Value

A new instance of OSSerialize with a retain count of 1; `NULL` on failure.

## Overview

The serializer will grow as needed to accommodate more data.

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

previouslySerialized

Checks whether the object has already been serialized into the XML stream, emitting a reference if it has.

text

Returns the XML text serialized so far.

