

- Create ML
- MLImageClassifier
- MLImageClassifier.DataSource
-  stratifiedSplit(proportions:seed:) 

Instance Method

# stratifiedSplit(proportions:seed:)

Generates an array of labeled image dictionaries by splitting the data source into strata.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
func stratifiedSplit(
    proportions: [Double],
    seed: Int = timestampSeed()
) throws -> [[String : [URL]]]
```

## Parameters 

`proportions`  

An array of proportions, each in the range `[0.0, 1.0]`.

`seed`  

A seed number for the random-number generator.

## Return Value

An array of dictionaries of labeled images.

## See Also

### Splitting the data

func stratifiedSplit&lt;RNG>(proportions: [Double], generator: inout RNG) throws -> [[String : [URL]]]

Generates an array of labeled image dictionaries by splitting the data source into strata using the random-number generator.

