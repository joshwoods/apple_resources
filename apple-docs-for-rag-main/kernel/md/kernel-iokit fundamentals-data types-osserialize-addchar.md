

- Kernel
- IOKit Fundamentals
- Data Types
- OSSerialize
-  addChar 

# addChar

Appends a single character to the XML stream.

``` source
virtual bool addChar(
 const charaChar); 
```

## Parameters 

`aChar`  

The character to append to the XML stream.

## Return Value

`true` if `char` is successfully added to the XML stream, `false` otherwise.

## See Also

### Miscellaneous

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

