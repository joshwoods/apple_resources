

- Security
-  kSecTransformErrorInvalidInputDictionary Deprecated

Global Variable

# kSecTransformErrorInvalidInputDictionary

A dictionary used to import a transform has invalid data.

macOS 10.7–13.0Deprecated

``` source
var kSecTransformErrorInvalidInputDictionary: CFIndex { get }
```

## Discussion

This error may occur when trying to import a transform from a data representation using the SecTransformCreateFromExternalRepresentation(_:_:) function.

