

- Create ML
- MLTextClassifier
-  write(to:metadata:) 

Instance Method

# write(to:metadata:)

Exports the text classifier as a Core ML model file at the specified URL.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
func write(
    to fileURL: URL,
    metadata: MLModelMetadata? = nil
) throws
```

## Parameters 

`fileURL`  

The location in the file system to which the file should be written.

`metadata`  

Descriptive information to include with the exported model file.

## Mentioned in 

Creating a text classifier model

Creating a Text Classifier Model

## See Also

### Saving a text classifier

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the text classifier as a Core ML model file at the specified file path.

