

- Core Foundation
-  CFXMLParserEndXMLStructureCallBack 

Type Alias

# CFXMLParserEndXMLStructureCallBack

Callback function invoked by the parser to notify your application that an XML structure (and all its children) have been completely parsed.

macOS

``` source
typealias CFXMLParserEndXMLStructureCallBack = (CFXMLParser?, UnsafeMutableRawPointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`parser`  

The CFXMLParser object making the callback.

`xmlType`  

The program-defined value representing the XML element whose end tag has been detected. This value was returned by the CFXMLParserCreateXMLStructureCallBack callback.

`info`  

The program-defined context data you specified in the CFXMLParserContext structure when creating the parser.

## Discussion

As elements are encountered, this callback is called first, then the CFXMLParserAddChildCallBack callback to add the new structure to its parent, then the CFXMLParserAddChildCallBack callback (potentially several times) to add the new structure’s children to it, and then finally the CFXMLParserEndXMLStructureCallBack callback to show that the structure has been fully parsed.This callback is optional.

## See Also

### Callbacks

typealias CFXMLParserAddChildCallBack

Callback function invoked by the parser to notify your application of parent/child relationships between XML structures.

typealias CFXMLParserCopyDescriptionCallBack

Callback function invoked by the parser when handling the information pointer.

typealias CFXMLParserCreateXMLStructureCallBack

Callback function invoked when the parser encounters an XML open tag.

typealias CFXMLParserHandleErrorCallBack

Callback function invoked by the parser to notify your application that an error has occurred.

typealias CFXMLParserReleaseCallBack

Callback function invoked by the parser when it wants to release a reference to the information pointer.

typealias CFXMLParserResolveExternalEntityCallBack

Callback function invoked by the parser to notify your application that an external entity has been referenced.

typealias CFXMLParserRetainCallBack

Callback function invoked by the parser when it needs another reference to the information pointer.

