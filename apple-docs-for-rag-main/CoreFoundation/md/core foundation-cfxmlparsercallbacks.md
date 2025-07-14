

- Core Foundation
-  CFXMLParserCallBacks 

Structure

# CFXMLParserCallBacks

Contains version information and function pointers to callbacks needed when parsing XML.

macOS

``` source
struct CFXMLParserCallBacks
```

## Overview

This structure is passed to one of the `CFXMLParserCreate...` functions. Only the `createXMLStructure`, `addChild`, and `endXMLStructure` fields are required. Set the others to `NULL` if you don’t wish to implement them.

## Topics

### Initializers

init()

init(version: CFIndex, createXMLStructure: CFXMLParserCreateXMLStructureCallBack!, addChild: CFXMLParserAddChildCallBack!, endXMLStructure: CFXMLParserEndXMLStructureCallBack!, resolveExternalEntity: CFXMLParserResolveExternalEntityCallBack!, handleError: CFXMLParserHandleErrorCallBack!)

### Instance Properties

var addChild: CFXMLParserAddChildCallBack!

Called when a child is added.

var createXMLStructure: CFXMLParserCreateXMLStructureCallBack!

Called when an XML structure is created.

var endXMLStructure: CFXMLParserEndXMLStructureCallBack!

Called when an XML structure has ended.

var handleError: CFXMLParserHandleErrorCallBack!

Called when a parse error needs to be handled.

var resolveExternalEntity: CFXMLParserResolveExternalEntityCallBack!

Called when an external entity needs to be resolved.

var version: CFIndex

Version number. Must be `0`.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

struct CFXMLParserContext

Contains version information and function pointers to callbacks used when handling a program-defined context.

