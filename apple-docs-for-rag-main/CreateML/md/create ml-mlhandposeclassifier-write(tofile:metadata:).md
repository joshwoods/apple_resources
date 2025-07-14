

- Create ML
- MLHandPoseClassifier
-  write(toFile:metadata:) 

Instance Method

# write(toFile:metadata:)

Exports the hand pose classifier as a Core ML model file.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
func write(
    toFile path: String,
    metadata: MLModelMetadata? = nil
) throws
```

## Parameters 

`path`  

A file-system path.

`metadata`  

The model’s description, author, version, and license information.

## See Also

### Saving a hand pose classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the hand pose classifier as a CoreML model file.

