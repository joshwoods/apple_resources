

- Create ML
- MLTextClassifier
-  write(toFile:metadata:) 

Instance Method

# write(toFile:metadata:)

Exports the text classifier as a Core ML model file at the specified file path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
func write(
    toFile path: String,
    metadata: MLModelMetadata? = nil
) throws
```

## Parameters 

`path`  

A file system path where the model file should be written.

`metadata`  

Descriptive information to include with the exported model file.

## See Also

### Saving a text classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the text classifier as a Core ML model file at the specified URL.

