

- Create ML
- MLImageClassifier
-  MLImageClassifier.DataSource 

Enumeration

# MLImageClassifier.DataSource

A data source for an image classifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
enum DataSource
```

## Mentioned in 

Creating an Image Classifier Model

## Overview

Use a data source to provide training or testing data to an image classifier.

To train a model programmatically with an MLImageClassifier instance, initialize a data source with the URL of the directory that contains the data. Use either MLImageClassifier.DataSource.labeledDirectories(at:) or MLImageClassifier.DataSource.labeledFiles(at:) to do this, depending on whether your images are grouped by directory or by file name. See the respective creation methods for details about how to arrange your image files in each case.

When you train a model using `MLImageClassifierBuilder`, you don’t initialize a data source directly. Instead, you drag the directory containing your data from a Finder window into the live view. The builder automatically chooses the correct kind of data source based on how your images are arranged inside that directory, looking for either labeled directories or labeled files.

## Topics

### Creating a data source

case labeledDirectories(at: URL)

An image classifier data source that uses the directory structure to label images.

case labeledFiles(at: URL)

An image classifier data source that uses file names to label images.

### Retrieving the data

func labeledImages() throws -> [String : [URL]]

Returns the labeled images represented by the data source.

case filesByLabel([String : [URL]])

Dictionary of labels to file URLs.

### Splitting the data

func stratifiedSplit(proportions: [Double], seed: Int) throws -> [[String : [URL]]]

Generates an array of labeled image dictionaries by splitting the data source into strata.

func stratifiedSplit&lt;RNG>(proportions: [Double], generator: inout RNG) throws -> [[String : [URL]]]

Generates an array of labeled image dictionaries by splitting the data source into strata using the random-number generator.

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting types

struct ModelParameters

Parameters that affect the process of training an image classifier model.

