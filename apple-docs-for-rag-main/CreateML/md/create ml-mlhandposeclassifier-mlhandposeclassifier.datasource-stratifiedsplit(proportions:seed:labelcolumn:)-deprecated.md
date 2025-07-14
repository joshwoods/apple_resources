

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.DataSource
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

## Discussion

- proportions: An array of stratum proportions, each in the range `[0.0, 1.0]`.

  - seed: A seed number for the random-number generator.

- labelColumn: The name of the column or category the method uses to stratify the contents of the data source.

## See Also

### Exporting a data source

func labeledMedia() throws -> [String : [URL]]

Generates a dictionary that contains the data source’s classification labels paired with an array of URLs to the label’s image files.

func imagesWithAnnotations() throws -> MLDataTable

Generates a data table that contains a column for the data source’s image file URLs and a column of annotations.

Deprecated

func keypointsWithAnnotations() throws -> MLDataTable

Generates a data table that contains a column for hand joint locations and hand pose annotations.

Deprecated

