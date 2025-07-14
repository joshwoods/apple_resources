

- Core Services
- Carbon Core
- Carbon Core Structures
-  ccntTokenRecord 

Structure

# ccntTokenRecord

Stores token information used by the AEResolve functionwhile locating a range of objects.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct ccntTokenRecord
```

## Overview

When the AEResolve(_:_:_:) functioncalls an object accessor function to locate a range of objects, theApple Event Manager replaces the descriptor of type `typeCurrentContainer` witha token for the container of each boundary object. When using `AEResolve` toresolve the object specifier, your application doesn’t need toexamine the contents of this token, because the Apple Event Managerkeeps track of it.

If your application attempts to resolve some or all of theobject specifier without calling `AEResolve`,the application may need to examine the token before it can locatethe boundary objects. The token provided by the Apple Event Managerfor a boundary object’s container is a descriptor of type `typeToken` whosedata storage pointer refers to a structure of type `ccntTokenRecord`.

## Topics

### Initializers

init()

init(tokenClass: DescType, token: AEDesc)

### Instance Properties

var token: AEDesc

A token for the current container. (Token is definedin AEDisposeToken(_:). See AEDesc.

var tokenClass: DescType

The class ID of the container represented by the `token` parameter.See DescType.

