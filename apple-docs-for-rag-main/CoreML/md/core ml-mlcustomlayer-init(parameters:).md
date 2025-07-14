

- Core ML
- MLCustomLayer
-  init(parameters:) 

Initializer

# init(parameters:)

Initializes the custom layer implementation.

iOS 11.2+iPadOS 11.2+Mac Catalyst 13.1+macOS 10.13.2+tvOS 11.2+visionOS 1.0+watchOS 4.2+

``` source
init(parameters: [String : Any]) throws
```

**Required**

## Parameters 

`parameters`  

The contents of the parameter dictionary from the `.mlmodel` file.

## Mentioned in 

Creating and Integrating a Model with Custom Layers

## Discussion

Implement this method to initialize your custom layer. It is called once, at load time. Use the parameters to configure the custom layer as needed.

If the layer cannot be initialized, your implementation should throw a customLayer error.

