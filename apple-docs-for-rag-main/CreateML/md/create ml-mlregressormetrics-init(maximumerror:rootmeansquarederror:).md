

- Create ML
- MLRegressorMetrics
-  init(maximumError:rootMeanSquaredError:) 

Initializer

# init(maximumError:rootMeanSquaredError:)

Creates regressor metrics describing the quality of your model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(
    maximumError: Double,
    rootMeanSquaredError: Double
)
```

## Parameters 

`maximumError`  

The maximum error of the model for the training data.

`rootMeanSquaredError`  

The root mean squared error of the model for the training data.

## Discussion

You typically don’t initialize metrics directly. Instead you get metrics about your model after training. For example, when you train an MLRegressor, you can look at its trainingMetrics and validationMetrics properties. Additionally, you can check the performance on a test set with the evaluation(on:) method.

