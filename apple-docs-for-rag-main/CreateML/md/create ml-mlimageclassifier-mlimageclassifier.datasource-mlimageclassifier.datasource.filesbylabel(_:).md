

- Create ML
- MLImageClassifier
- MLImageClassifier.DataSource
-  MLImageClassifier.DataSource.filesByLabel(\_:) 

Case

# MLImageClassifier.DataSource.filesByLabel(\_:)

Dictionary of labels to file URLs.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
case filesByLabel([String : [URL]])
```

## See Also

### Retrieving the data

func labeledImages() throws -> [String : [URL]]

Returns the labeled images represented by the data source.

