

- Create ML
- MLHandPoseClassifier
-  write(to:metadata:) 

Instance Method

# write(to:metadata:)

Exports the hand pose classifier as a CoreML model file.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
func write(
    to fileURL: URL,
    metadata: MLModelMetadata? = nil
) throws
```

## Parameters 

`fileURL`  

A file-system URL.

`metadata`  

The model’s description, author, version, and license information.

## See Also

### Saving a hand pose classifier

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the hand pose classifier as a Core ML model file.

