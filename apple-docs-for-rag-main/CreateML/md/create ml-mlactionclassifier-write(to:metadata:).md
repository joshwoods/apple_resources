

- Create ML
- MLActionClassifier
-  write(to:metadata:) 

Instance Method

# write(to:metadata:)

Exports the action classifier as a Core ML model file to a location in the file system.

macOS 11.0+

``` source
func write(
    to fileURL: URL,
    metadata: MLModelMetadata? = nil
) throws
```

## Discussion

- fileURL: The location URL in the file system where you want to save the model.

- metadata: Descriptive information to include with the exported model file.

## See Also

### Saving an action classifier

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the action classifier as a Core ML model file to the file path.

