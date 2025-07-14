

- Create ML
- MLTextClassifier
- MLTextClassifier.DataSource
-  stratifiedSplit(proportions:seed:labelColumn:textColumn:) 

Instance Method

# stratifiedSplit(proportions:seed:labelColumn:textColumn:)

Generates a data table by splitting the data source into strata.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 10.14–14.0DeprecatedvisionOS 1.0+

``` source
func stratifiedSplit(
    proportions: [Double],
    seed: Int = timestampSeed(),
    labelColumn: String,
    textColumn: String
) throws -> MLDataTable
```

## Parameters 

`proportions`  

An array of proportions, each in the range `[0.0, 1.0]`.

`seed`  

A seed number for the random-number generator. The default value is the current epoch time in milliseconds.

`labelColumn`  

The name of the column with the labels.

`textColumn`  

The name of the column with the text data.

## Return Value

A new data table.

## See Also

### Retrieving the data

func labeledTexts() throws -> [String : [String]]

Fetches the labeled data from the data source.

