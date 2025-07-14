

- Create ML
- MLTextClassifier
- MLTextClassifier.DataSource
-  labeledTexts() 

Instance Method

# labeledTexts()

Fetches the labeled data from the data source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
func labeledTexts() throws -> [String : [String]]
```

## Return Value

A dictionary that contains each label with their related text entries.

## See Also

### Retrieving the data

func stratifiedSplit(proportions: [Double], seed: Int, labelColumn: String, textColumn: String) throws -> MLDataTable

Generates a data table by splitting the data source into strata.

