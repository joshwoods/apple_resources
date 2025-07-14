

- Create ML
- MLHandActionClassifier
-  write(toFile:metadata:) 

Instance Method

# write(toFile:metadata:)

Exports the hand action classifier as a Core ML model file.

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

### Saving a hand action classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the hand action classifier as a CoreML model file.

