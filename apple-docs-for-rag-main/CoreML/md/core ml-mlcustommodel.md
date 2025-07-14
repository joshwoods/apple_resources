

- Core ML
-  MLCustomModel 

Protocol

# MLCustomModel

An interface that defines the behavior of a custom model.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
protocol MLCustomModel
```

## Overview

To integrate your custom model with Core ML, adopt the MLCustomModel protocol in the implementation of your custom model. If you use a Swift class for your custom implementation, make it accessible to Core ML by using the `@objc(`*name*`)` attribute.

```
@objc(MyCustomModel)
class MyCustomModel: NSObject, MLCustomModel {
  ...
}
```

This defines the Objective-C name for the class, which Core ML needs to access your custom class’s implementation.

## Topics

### Creating the Model

init(modelDescription: MLModelDescription, parameters: [String : Any]) throws

Creates a custom model with the given description and parameters.

**Required**

### Making Predictions

func prediction(from: any MLFeatureProvider, options: MLPredictionOptions) throws -> any MLFeatureProvider

Predicts output values from the given input features.

**Required**

func predictions(from: any MLBatchProvider, options: MLPredictionOptions) throws -> any MLBatchProvider

Predicts output values from the given batch of input features.

