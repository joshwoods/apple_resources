

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.DataSource
-  imagesWithAnnotations() Deprecated

Instance Method

# imagesWithAnnotations()

Generates a data table that contains a column for the data source’s image file URLs and a column of annotations.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedvisionOS 1.0+

``` source
func imagesWithAnnotations() throws -> MLDataTable
```

Deprecated

Use gatherAnnotatedFileNames()

## See Also

### Exporting a data source

func labeledMedia() throws -> [String : [URL]]

Generates a dictionary that contains the data source’s classification labels paired with an array of URLs to the label’s image files.

func keypointsWithAnnotations() throws -> MLDataTable

Generates a data table that contains a column for hand joint locations and hand pose annotations.

Deprecated

func stratifiedSplit(proportions: [Double], seed: Int, labelColumn: String) throws -> MLDataTable

Generates a data table by splitting the data source into strata.

Deprecated

