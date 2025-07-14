

- Core Foundation
-  CFXMLParserHandleErrorCallBack 

Type Alias

# CFXMLParserHandleErrorCallBack

Callback function invoked by the parser to notify your application that an error has occurred.

macOS

``` source
typealias CFXMLParserHandleErrorCallBack = (CFXMLParser?, CFXMLParserStatusCode, UnsafeMutableRawPointer?) -> DarwinBoolean
```

## Parameters 

`parser`  

A CFXMLParser object making the callback.

`error`  

A status code describing the error.

`info`  

The program-defined context data you specified in the CFXMLParserContext structure when creating the parser.

## Return Value

`true` if the parser should continue parsing the XML, `false` if the parser should stop.

## Discussion

If this callback is not defined, the parser will silently attempt to recover. Otherwise, this callback may return false to force the parser to stop. If this callback returns true, the parser will attempt to recover (fatal errors will still cause the parse to abort immediately). This callback is optional.

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

typealias CFXMLParserReleaseCallBack

Callback function invoked by the parser when it wants to release a reference to the information pointer.

typealias CFXMLParserResolveExternalEntityCallBack

Callback function invoked by the parser to notify your application that an external entity has been referenced.

typealias CFXMLParserRetainCallBack

Callback function invoked by the parser when it needs another reference to the information pointer.

