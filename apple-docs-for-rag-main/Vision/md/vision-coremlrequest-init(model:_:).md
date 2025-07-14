

- Vision
- CoreMLRequest
-  init(model:\_:) 

Initializer

# init(model:\_:)

Creates a Core ML request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
init(
    model: CoreMLModelContainer,
    _ revision: CoreMLRequest.Revision? = nil
)
```

## Parameters 

`model`  

The container for a Core ML model.

`revision`  

The specific algorithm or implementation that the framework uses to perform the request.

