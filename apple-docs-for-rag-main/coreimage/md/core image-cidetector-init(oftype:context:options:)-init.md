

- Core Image
- CIDetector
-  init(ofType:context:options:) 

Initializer

# init(ofType:context:options:)

Creates and returns a configured detector.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
init?(
    ofType type: String,
    context: CIContext?,
    options: [String : Any]? = nil
)
```

## Parameters 

`type`  

A string indicating the kind of detector you are interested in. See Detector Types.

`context`  

A Core Image context that the detector can use when analyzing an image.

`options`  

A dictionary containing details on how you want the detector to be configured. See Detector Configuration Keys.

## Return Value

A configured detector.

## Discussion

A CIDetector object can potentially create and hold a significant amount of resources. Where possible, reuse the same `CIDetector` instance. Also, when processing images with a detector object, your application performs better if the CIContext used to initialize the detector is the same context used to process the ciImage objects.

