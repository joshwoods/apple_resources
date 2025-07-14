

- Core Foundation
- CFXMLParserCallBacks
-  init(version:createXMLStructure:addChild:endXMLStructure:resolveExternalEntity:handleError:) 

Initializer

# init(version:createXMLStructure:addChild:endXMLStructure:resolveExternalEntity:handleError:)

macOS

``` source
init(
    version: CFIndex,
    createXMLStructure: CFXMLParserCreateXMLStructureCallBack!,
    addChild: CFXMLParserAddChildCallBack!,
    endXMLStructure: CFXMLParserEndXMLStructureCallBack!,
    resolveExternalEntity: CFXMLParserResolveExternalEntityCallBack!,
    handleError: CFXMLParserHandleErrorCallBack!
)
```

