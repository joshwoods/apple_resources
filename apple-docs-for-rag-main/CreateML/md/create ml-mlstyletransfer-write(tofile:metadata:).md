

- Create ML
- MLStyleTransfer
-  write(toFile:metadata:) 

Instance Method

# write(toFile:metadata:)

Exports the style transfer model as a Core ML model file to the file path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
func write(
    toFile path: String,
    metadata: MLModelMetadata? = .init()
) throws
```

## Discussion

- path: The location path in the file system where you want to save the model.

- metadata: Descriptive information to include with the exported model file.

## See Also

### Saving a style transfer model

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the style transfer model as a Core ML model file to a location in the file system.

