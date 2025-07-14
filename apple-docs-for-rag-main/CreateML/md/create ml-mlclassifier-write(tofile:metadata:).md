

- Create ML
- MLClassifier
-  write(toFile:metadata:) 

Instance Method

# write(toFile:metadata:)

Exports a Core ML model file for use in your app.

macOS 10.14+

``` source
func write(
    toFile path: String,
    metadata: MLModelMetadata?
) throws
```

## See Also

### Saving a classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

