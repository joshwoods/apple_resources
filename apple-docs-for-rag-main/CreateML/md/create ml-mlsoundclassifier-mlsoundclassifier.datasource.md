

- Create ML
- MLSoundClassifier
-  MLSoundClassifier.DataSource 

Enumeration

# MLSoundClassifier.DataSource

A representation of a sound-classifier dataset located in the file system or in a data table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
enum DataSource
```

## Overview

Use a data source to represent a dataset for training, validating, or testing a sound classifier.

## Topics

### Creating a data source

case labeledDirectories(at: URL)

Creates a data source from a folder with subfolders that each contain audio files.

case labeledFiles(at: URL)

Creates a data source from a folder that contains audio files, each named after the sound they represent.

case filesByLabel([String : [URL]])

Creates a data source from a dictionary.

case features(table: MLDataTable, featureColumn: String, labelColumn: String, parameters: MLSoundClassifier.FeatureExtractionParameters)

Creates a data source from a data table of audio features.

case featuresDataFrame(DataFrame, featureColumn: String, labelColumn: String, parameters: MLSoundClassifier.FeatureExtractionParameters)

Creates a data source from a data frame of audio features.

struct FeatureExtractionParameters

Parameters that affect the process of extracting sound features from audio files.

### Retrieving the data

func labeledSounds() throws -> [String : [URL]]

Generates a dictionary of the data source’s labeled audio files.

### Partitioning the data

func stratifiedSplit(proportions: [Double], seed: Int) throws -> [[String : [URL]]]

Generates an array of labeled audio dictionaries by splitting the data source into strata.

func stratifiedSplit&lt;RNG>(proportions: [Double], generator: inout RNG) throws -> [[String : [URL]]]

Generates an array of labeled audio dictionaries by splitting the data source into strata using the random-number generator.

## See Also

### Supporting types

struct ModelParameters

Parameters that affect the process of training a sound-classifier model.

