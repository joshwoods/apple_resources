

- Create ML
- MLActionClassifier
-  write(toFile:metadata:) 

Instance Method

# write(toFile:metadata:)

Exports the action classifier as a Core ML model file to the file path.

macOS 11.0+

``` source
func write(
    toFile path: String,
    metadata: MLModelMetadata? = nil
) throws
```

## Discussion

- path : The location path in the file system where you want to save the model.

- metadata: Descriptive information to include with the exported model file.

## See Also

### Saving an action classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the action classifier as a Core ML model file to a location in the file system.

