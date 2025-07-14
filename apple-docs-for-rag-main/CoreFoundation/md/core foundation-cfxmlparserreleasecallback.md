

- Core Foundation
-  CFXMLParserReleaseCallBack 

Type Alias

# CFXMLParserReleaseCallBack

Callback function invoked by the parser when it wants to release a reference to the information pointer.

macOS

``` source
typealias CFXMLParserReleaseCallBack = (UnsafeRawPointer?) -> Void
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

typealias CFXMLParserResolveExternalEntityCallBack

Callback function invoked by the parser to notify your application that an external entity has been referenced.

typealias CFXMLParserRetainCallBack

Callback function invoked by the parser when it needs another reference to the information pointer.

