

- Security
-  SecTransformCopyExternalRepresentation(\_:) Deprecated

Function

# SecTransformCopyExternalRepresentation(\_:)

Creates a dictionary that contains enough information to be able to recreate a transform.

macOS 10.7–12.0Deprecated

``` source
func SecTransformCopyExternalRepresentation(_ transformRef: SecTransform) -> CFDictionary
```

Deprecated

SecTransform is no longer supported

## Parameters 

`transformRef`  

The transformRef to be externalized.

## Discussion

This function returns a CFDictionaryRef that contains sufficient information to be able to recreate this transform. You can pass this CFDictionaryRef to SecTransformCreateFromExternalRepresentation to be able to recreate the transform. The dictionary can also be written out to disk using the techniques described here.

http://developer.apple.com/mac/library/documentation/CoreFoundation/Conceptual/CFPropertyLists/Articles/Saving.html

