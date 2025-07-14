

- Create ML
- MLSoundClassifier
- MLSoundClassifier.DataSource
-  stratifiedSplit(proportions:seed:) 

Instance Method

# stratifiedSplit(proportions:seed:)

Generates an array of labeled audio dictionaries by splitting the data source into strata.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

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

A seed for the random-number generator.

## Return Value

An array of dictionaries of labeled audio files. Each dictionary key is a label string and its value is an array of audio-file URLs.

## See Also

### Partitioning the data

func stratifiedSplit&lt;RNG>(proportions: [Double], generator: inout RNG) throws -> [[String : [URL]]]

Generates an array of labeled audio dictionaries by splitting the data source into strata using the random-number generator.

