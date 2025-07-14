

- Create ML
- MLBoostedTreeClassifier
-  write(to:metadata:) 

Instance Method

# write(to:metadata:)

Exports a Core ML model file for use in your app.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func write(
    to fileURL: URL,
    metadata: MLModelMetadata? = nil
) throws
```

## See Also

### Saving a boosted tree classifier

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

