

- Kernel
- IOKit Fundamentals
- Data Types
- OSSerialize
-  clearText 

# clearText

Resets the OSSerialize object.

``` source
virtual void clearText(); 
```

## Overview

This function is a useful optimization if you are serializing the same object repeatedly.

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

previouslySerialized

Checks whether the object has already been serialized into the XML stream, emitting a reference if it has.

text

Returns the XML text serialized so far.

withCapacity

Creates and initializes an empty OSSerialize object.

