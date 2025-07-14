

- Kernel
- IOKit Fundamentals
- Data Types
- OSSerialize
-  text 

# text

Returns the XML text serialized so far.

``` source
virtual char * text() const; 
```

## Return Value

The nul-terminated XML data serialized so far.

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

withCapacity

Creates and initializes an empty OSSerialize object.

