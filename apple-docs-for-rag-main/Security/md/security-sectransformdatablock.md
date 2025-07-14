

- Security
-  SecTransformDataBlock 

Type Alias

# SecTransformDataBlock

A block used to override the default data handling for a transform.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias SecTransformDataBlock = (CFTypeRef) -> Unmanaged?
```

## Parameters 

`data`  

The data to be processed. When this block is used to to implement the kSecTransformActionProcessData action, the data is the input data that is to be processed into the output data. When this block is used to implement the kSecTransformActionInternalizeExtraData action, the data is a CFDictionary that contains the data that needs to be imported.

## Return Value

`NULL` for the kSecTransformActionInternalizeExtraData action, the data to be passed to the output attribute for any other action, or a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 instance on failure.

