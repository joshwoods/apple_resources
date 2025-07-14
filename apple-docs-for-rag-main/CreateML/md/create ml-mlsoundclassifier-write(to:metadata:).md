

- Create ML
- MLSoundClassifier
-  write(to:metadata:) 

Instance Method

# write(to:metadata:)

Exports the sound classifier as a model file to a location in the file system.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
func write(
    to fileURL: URL,
    metadata: MLModelMetadata? = nil
) throws
```

## Parameters 

`fileURL`  

The location URL in the file system where you want to save the model.

`metadata`  

Descriptive information to include with the exported model file.

## Discussion

Use this method to save the sound classifier as a Core ML model to a URL.

This method:

- Uses the name `SoundClassifier.mlmodel` if the URL’s location is a directory

- Appends `mlmodel` as the extension if you don’t provide one

- Creates intermediate directories if none exist

## See Also

### Saving a sound classifier

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the sound classifier as a model file to a path in the file system.

