

- Create ML
- MLObjectDetector
- MLObjectDetector.DataSource
-  gatherAnnotatedFileNames() 

Instance Method

# gatherAnnotatedFileNames()

Processes the data source and returns a data frame that contains file URLs and annotations.

macOS 14.0+

``` source
func gatherAnnotatedFileNames() throws -> DataFrame
```

## Discussion

This method collects file names from the filesystem if necessary. If the data source is already in table format it renames the columns to the default column names.

