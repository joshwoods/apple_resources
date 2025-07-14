

- Core ML
- Model Customization
-  Creating and Integrating a Model with Custom Layers 

Article

# Creating and Integrating a Model with Custom Layers

Add models with custom neural-network layers to your app.

## Overview

New network layers and architectures solve problems that might be difficult or impractical with code. You can support each new layer type before Core ML directly supports it by implementing a *custom layer*. A custom layer is a class that adopts MLCustomLayer and implements the methods to run a neural network layer in code.

Note

Core ML supports models with custom layers beginning with these software releases: iOS 11.2, macOS 10.13.2, tvOS 11.2 and watchOS 4.2.

### Add a Model You Acquire or Create

If you have a Core ML model with custom layers, add the model to your Xcode project.

Otherwise, convert a third-party model and designate the new layers as custom with the Core ML Tools. Follow the steps on the Custom Operators page to define the new layers as custom. Give each custom layer a unique name by assigning a unique string to the operator’s class name binding.

```
```

Save the Core ML model you converted and add it to your Xcode project.

### Integrate or Create a Class for Each Custom Layer

If the author of the model you plan to add to your Xcode project implemented the custom layers in source-code files, add the source files into your Xcode project.

Otherwise, implement each custom layer by creating a Swift or Objective-C class for each layer. Inspect the names of the model’s custom layers by opening the model in Xcode:

Create a class for each custom layer that the model has in its list of dependencies and name each class to match the custom layer it implements.

Important

Swift classes must subclass NSObject and use the `@objc` attribute so that Core ML can access your custom layer’s implementation.

Adopt the MLCustomLayer protocol by implementing the following:

init(parameters:)  
An initializer that configures the layer’s parameters that the model defines in its Core ML model file. Core ML initializes each layer once at load time.

setWeightData(_:)  
A method that configures the layer’s weights that the model defines in its Core ML model file. Core ML invokes this method once at load time, after initialization.

outputShapes(forInputShapes:)  
A method that defines the layer’s output shapes based on the input shapes at runtime. Core ML invokes this method at load time, after initialization, and again each time the layer’s input shapes change.

evaluate(inputs:outputs:)  
A method that defines the computational behavior for your custom layer. Core ML invokes this method each time your model makes a prediction on the CPU.

encode(commandBuffer:inputs:outputs:)  
An optional method that defines your layer’s computational behavior with GPU commands.

Core ML invokes the appropriate MLCustomLayer methods for each custom layer at runtime when your app calls the prediction(from:) method.

Warning

Don’t change the values that Core ML provides to these methods — such as weights, inputs, or outputs — because it may cause your app to behave in unexpected ways, and possibly crash.

### Test the Custom Layers

If applicable, test the custom layers by using the model to make predictions with input values from one or more test cases. Confirm the model layers function correctly by comparing the model’s prediction values to the output values for each test case.

## See Also

### Custom Model Layers

protocol MLCustomLayer

An interface that defines the behavior of a custom layer in your neural network model.

