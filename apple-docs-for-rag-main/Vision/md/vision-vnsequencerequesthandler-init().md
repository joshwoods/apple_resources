

- Vision
- VNSequenceRequestHandler
-  init() 

Initializer

# init()

Initializes a sequence request handler.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init()
```

## Discussion

Unlike the VNImageRequestHandler, this initializer accepts no input because image data and auxiliary parameters may change from frame to frame, and are handled dynamically in the request-handling `perform` methods.

