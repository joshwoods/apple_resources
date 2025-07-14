

- Create ML
- MLTextClassifier
- MLTextClassifier.DataSource
-  MLTextClassifier.DataSource.labeledDirectories(at:) 

Case

# MLTextClassifier.DataSource.labeledDirectories(at:)

A root directory of labeled directories for your data set.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
case labeledDirectories(at: URL)
```

## Discussion

Labeled directories can be used to organize textual inputs. Just like the data source used with the image classifier, place the collected text inputs of the same kind in a directory. Name that directory with the label appropriate for the textual inputs.

