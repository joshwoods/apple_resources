

- Create ML Components
- LogisticRegressionClassifier
-  init(labels:configuration:) 

Initializer

# init(labels:configuration:)

Creates a logistic regression classifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    labels: Set,
    configuration: LogisticRegressionClassifier.Configuration = Configuration()
)
```

## Parameters 

`labels`  

The labels used to train the classifier.

`configuration`  

The configuration.

## See Also

### Creating a classifier

struct Configuration

A logistic regression classifier configuration.

