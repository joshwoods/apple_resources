

- Create ML
- MLImageClassifier
-  write(toFile:metadata:) 

Instance Method

# write(toFile:metadata:)

Exports the image classifier as a Core ML model file to the file path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
func write(
    toFile path: String,
    metadata: MLModelMetadata? = nil
) throws
```

## Parameters 

`path`  

The location path in the file system where you want to save the model.

`metadata`  

Descriptive information to include with the exported model file.

## See Also

### Saving an image classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the image classifier as a Core ML model file to a location in the file system.

