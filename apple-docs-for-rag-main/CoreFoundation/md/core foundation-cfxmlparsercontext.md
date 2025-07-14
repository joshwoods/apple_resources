

- Core Foundation
-  CFXMLParserContext 

Structure

# CFXMLParserContext

Contains version information and function pointers to callbacks used when handling a program-defined context.

macOS

``` source
struct CFXMLParserContext
```

## Overview

You can associate a context with a parser when the parser is created. The context can be anything you wish and will be passed as a parameter to all of the XML parser callbacks.

## Topics

### Initializers

init()

init(version: CFIndex, info: UnsafeMutableRawPointer!, retain: CFXMLParserRetainCallBack!, release: CFXMLParserReleaseCallBack!, copyDescription: CFXMLParserCopyDescriptionCallBack!)

### Instance Properties

var copyDescription: CFXMLParserCopyDescriptionCallBack!

A copy description callback for your program-defined context data. Optional.

var info: UnsafeMutableRawPointer!

An arbitrary program-defined value passed to all the callbacks in this structure and in the CFXMLParserCallBacks structure.

var release: CFXMLParserReleaseCallBack!

A release callback for your program-defined context data. Optional.

var retain: CFXMLParserRetainCallBack!

A retain callback for your program-defined context data. Optional.

var version: CFIndex

Version number of this structure. Must be 0.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct CFXMLParserCallBacks

Contains version information and function pointers to callbacks needed when parsing XML.

