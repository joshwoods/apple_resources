

- Create ML
- MLImageClassifier
- MLImageClassifier.DataSource
-  stratifiedSplit(proportions:generator:) 

Instance Method

# stratifiedSplit(proportions:generator:)

Generates an array of labeled image dictionaries by splitting the data source into strata using the random-number generator.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
func stratifiedSplit(
    proportions: [Double],
    generator: inout RNG
) throws -> [[String : [URL]]] where RNG : RandomNumberGenerator
```

## Parameters 

`proportions`  

An array of proportions, each in the range `[0.0, 1.0]`.

`generator`  

A random-number generator.

## Return Value

An array of dictionaries of labeled images.

## See Also

### Splitting the data

func stratifiedSplit(proportions: [Double], seed: Int) throws -> [[String : [URL]]]

Generates an array of labeled image dictionaries by splitting the data source into strata.

