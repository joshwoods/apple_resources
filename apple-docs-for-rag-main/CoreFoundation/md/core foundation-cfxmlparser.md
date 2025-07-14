

- Core Foundation
-  CFXMLParser 

Class

# CFXMLParser

macOS

``` source
class CFXMLParser
```

## Overview

CFXMLParser provides an XML parser you can use to find and extract data in XML documents. You can use a high-level interface to load an XML document into a Core Foundation collection object. A low-level callback-based interface allows you to perform any action you wish on an XML structured type when it is detected by the parser. This opaque type is relevant for applications that need information about an XML document’s structure or content.

## Topics

### Callbacks

typealias CFXMLParserAddChildCallBack

Callback function invoked by the parser to notify your application of parent/child relationships between XML structures.

typealias CFXMLParserCopyDescriptionCallBack

Callback function invoked by the parser when handling the information pointer.

typealias CFXMLParserCreateXMLStructureCallBack

Callback function invoked when the parser encounters an XML open tag.

typealias CFXMLParserEndXMLStructureCallBack

Callback function invoked by the parser to notify your application that an XML structure (and all its children) have been completely parsed.

typealias CFXMLParserHandleErrorCallBack

Callback function invoked by the parser to notify your application that an error has occurred.

typealias CFXMLParserReleaseCallBack

Callback function invoked by the parser when it wants to release a reference to the information pointer.

typealias CFXMLParserResolveExternalEntityCallBack

Callback function invoked by the parser to notify your application that an external entity has been referenced.

typealias CFXMLParserRetainCallBack

Callback function invoked by the parser when it needs another reference to the information pointer.

### Data Types

struct CFXMLParserCallBacks

Contains version information and function pointers to callbacks needed when parsing XML.

struct CFXMLParserContext

Contains version information and function pointers to callbacks used when handling a program-defined context.

### Constants

struct CFXMLParserStatusCode

The various status and error flags that can be returned by the parser.

struct CFXMLParserOptions

Options you can use to control the parser’s treatment of an XML document.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

XML Programming Topics for Core Foundation

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

