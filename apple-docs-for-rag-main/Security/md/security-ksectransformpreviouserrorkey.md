

- Security
-  kSecTransformPreviousErrorKey 

Global Variable

# kSecTransformPreviousErrorKey

The key in an error’s `userInfo` dictionary whose value specifies the previous error when multiple errors occur during transform evaluation.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecTransformPreviousErrorKey: CFString
```

## Discussion

Use the value associated with this key to trace through a chain of doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 objects when more than one error occurs during transform evaluation.

