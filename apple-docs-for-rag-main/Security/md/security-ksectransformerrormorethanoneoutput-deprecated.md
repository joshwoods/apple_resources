

- Security
-  kSecTransformErrorMoreThanOneOutput Deprecated

Global Variable

# kSecTransformErrorMoreThanOneOutput

A transform has an internal routing error that has caused multiple outputs instead of a single discrete output.

macOS 10.7–13.0Deprecated

``` source
var kSecTransformErrorMoreThanOneOutput: CFIndex { get }
```

## Discussion

This error occurs if SecTransformExecute(_:_:) has already been called.

