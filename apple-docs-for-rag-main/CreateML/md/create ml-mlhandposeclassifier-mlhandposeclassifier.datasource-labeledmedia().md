

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.DataSource
-  labeledMedia() 

Instance Method

# labeledMedia()

Generates a dictionary that contains the data source’s classification labels paired with an array of URLs to the label’s image files.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
func labeledMedia() throws -> [String : [URL]]
```

## See Also

### Exporting a data source

func imagesWithAnnotations() throws -> MLDataTable

Generates a data table that contains a column for the data source’s image file URLs and a column of annotations.

Deprecated

func keypointsWithAnnotations() throws -> MLDataTable

Generates a data table that contains a column for hand joint locations and hand pose annotations.

Deprecated

func stratifiedSplit(proportions: [Double], seed: Int, labelColumn: String) throws -> MLDataTable

Generates a data table by splitting the data source into strata.

Deprecated

