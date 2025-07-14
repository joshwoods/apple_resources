

- Core Foundation
-  CFXMLParserRetainCallBack 

Type Alias

# CFXMLParserRetainCallBack

Callback function invoked by the parser when it needs another reference to the information pointer.

macOS

``` source
typealias CFXMLParserRetainCallBack = (UnsafeRawPointer?) -> UnsafeRawPointer?
```

## Parameters 

`info`  

The program-defined context data you specified in the CFXMLParserContext structure when creating the parser.

## See Also

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

