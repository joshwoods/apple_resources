

- Vision
- VNRequest
-  init(completionHandler:) 

Initializer

# init(completionHandler:)

Creates a new Vision request with an optional completion handler.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(completionHandler: VNRequestCompletionHandler? = nil)
```

## Parameters 

`completionHandler`  

The block to invoke after the request finishes processing.

## Discussion

Vision executes the completion handler on the same queue that it executes the request; however, this queue differs from the one where you called perform(_:).

## See Also

### Initializing a Request

convenience init()

Creates a new Vision request with no completion handler.

