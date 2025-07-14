

- Create ML
- MLSoundClassifier
- MLSoundClassifier.DataSource
-  stratifiedSplit(proportions:generator:) 

Instance Method

# stratifiedSplit(proportions:generator:)

Generates an array of labeled audio dictionaries by splitting the data source into strata using the random-number generator.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

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

An array of dictionaries of labeled audio files. Each dictionary key is a label string and its value is an array of audio-file URLs.

## See Also

### Partitioning the data

func stratifiedSplit(proportions: [Double], seed: Int) throws -> [[String : [URL]]]

Generates an array of labeled audio dictionaries by splitting the data source into strata.

