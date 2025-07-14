

- Core Foundation
-  CFXMLParserResolveExternalEntityCallBack 

Type Alias

# CFXMLParserResolveExternalEntityCallBack

Callback function invoked by the parser to notify your application that an external entity has been referenced.

macOS

``` source
typealias CFXMLParserResolveExternalEntityCallBack = (CFXMLParser?, UnsafeMutablePointer?, UnsafeMutableRawPointer?) -> Unmanaged?
```

## Parameters 

`parser`  

The CFXMLParser object making the callback.

`extID`  

The identifier for the external entity.

`info`  

The program-defined context data you specified in the CFXMLParserContext structure when creating the parser.

## Return Value

The external entity or `NULL` if it should not be resolved.

## Discussion

If this callback is not defined, the parser uses its internal routines to try and resolve the entity. Otherwise, if this callback returns NULL, a place holder for the external entity is inserted into the tree. In this manner, the parser’s client can prevent any external network or file accesses. This callback is optional.

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

typealias CFXMLParserRetainCallBack

Callback function invoked by the parser when it needs another reference to the information pointer.

