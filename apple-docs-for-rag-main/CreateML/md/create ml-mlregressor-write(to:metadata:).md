

- Create ML
- MLRegressor
-  write(to:metadata:) 

Instance Method

# write(to:metadata:)

Exports a Core ML model file for use in your app.

macOS 10.14+

``` source
func write(
    to fileURL: URL,
    metadata: MLModelMetadata?
) throws
```

## See Also

### Saving a regressor

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

