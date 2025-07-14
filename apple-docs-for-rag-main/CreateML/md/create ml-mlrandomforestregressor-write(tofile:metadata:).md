

- Create ML
- MLRandomForestRegressor
-  write(toFile:metadata:) 

Instance Method

# write(toFile:metadata:)

Exports a Core ML model file for use in your app.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func write(
    toFile path: String,
    metadata: MLModelMetadata? = nil
) throws
```

## See Also

### Saving a Random Forest Regressor

func write(to: URL, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

