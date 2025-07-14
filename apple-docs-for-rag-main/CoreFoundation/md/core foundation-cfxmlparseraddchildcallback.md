

- Core Foundation
-  CFXMLParserAddChildCallBack 

Type Alias

# CFXMLParserAddChildCallBack

Callback function invoked by the parser to notify your application of parent/child relationships between XML structures.

macOS

``` source
typealias CFXMLParserAddChildCallBack = (CFXMLParser?, UnsafeMutableRawPointer?, UnsafeMutableRawPointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`parser`  

The CFXMLParser object making the callback.

`parent`  

The program-defined value representing the XML element to whom `child` is being added. This value was returned by the CFXMLParserCreateXMLStructureCallBack callback when this element’s open tag was detected.

`child`  

The program-defined value representing the XML element that is being added to `parent`. This value was returned by the CFXMLParserCreateXMLStructureCallBack callback when this element’s open tag was detected.

`info`  

The program-defined context data you specified in the CFXMLParserContext structure when creating the parser.

## Discussion

If the CFXMLParserCreateXMLStructureCallBack function returns NULL for a given structure, that structure is omitted entirely, and this callback will *not* be called for either a NULL child or parent.

## See Also

### Callbacks

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

