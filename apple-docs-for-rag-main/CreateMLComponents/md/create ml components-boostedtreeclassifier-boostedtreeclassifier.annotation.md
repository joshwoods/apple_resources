

- Create ML Components
- BoostedTreeClassifier
-  BoostedTreeClassifier.Annotation 

Type Alias

# BoostedTreeClassifier.Annotation

The annotation type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Annotation = Label
```

## See Also

### Fitting the classifier

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> TreeClassifierModel&lt;Label>

Fits a boosted tree classifier model to a collection of examples.

typealias Transformer

The transformer type created by this estimator.

