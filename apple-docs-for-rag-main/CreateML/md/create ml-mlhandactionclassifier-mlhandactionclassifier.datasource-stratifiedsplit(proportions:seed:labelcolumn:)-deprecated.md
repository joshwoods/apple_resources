

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.DataSource
-  stratifiedSplit(proportions:seed:labelColumn:) Deprecated

Instance Method

# stratifiedSplit(proportions:seed:labelColumn:)

Generates a data table by splitting the data source into strata.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedvisionOS 1.0+

``` source
func stratifiedSplit(
    proportions: [Double],
    seed: Int = timestampSeed(),
    labelColumn: String
) throws -> MLDataTable
```

Deprecated

Use DataFrame.stratifiedSplit(on:by:)

## Parameters 

`proportions`  

An array of proportions, each in the range `[0.0, 1.0]`.

`seed`  

A seed number for the random-number generator.

`labelColumn`  

The name of the column that you want to stratify.

## Return Value

A new data table.

## See Also

### Exporting a data source

func labeledMedia() throws -> [String : [URL]]

Generates a dictionary that contains the data source’s classification labels paired with an array of URLs to the label’s video files.

func videosWithAnnotations() throws -> MLDataTable

Generates a data table that contains a column for the data source’s video file URLs and a column of annotations.

Deprecated

func keypointsWithAnnotations(targetFrameRate: Double) throws -> MLDataTable

Generates a data table that contains a column for hand joint locations and a column of hand action annotations.

Deprecated

func extractKeypoints(targetFrameRate: Double) throws -> DataFrame

Extracts key points from video files if necessary.

func gatherAnnotatedFileNames() throws -> DataFrame?

Processes the data source and returns a data frame that contains file URLs and annotations.

