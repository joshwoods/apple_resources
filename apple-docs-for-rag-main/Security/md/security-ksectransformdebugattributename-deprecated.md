

- Security
-  kSecTransformDebugAttributeName Deprecated

Global Variable

# kSecTransformDebugAttributeName

A write stream that should receive debug data.

macOS 10.7–12.0Deprecated

``` source
let kSecTransformDebugAttributeName: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

Set this attribute to a CFWriteStream. This signals the transform to write debugging information to the stream. If you set this attribute to kCFBooleanTrue, debug data is written to `stderr` instead.

