

- MapKit
- MKDirections
-  cancel() 

Instance Method

# cancel()

Cancels a pending request.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func cancel()
```

## Discussion

After canceling a request, you can call the calculate(completionHandler:) method again (if you want) to restart the request process.

## See Also

### Managing the request

var isCalculating: Bool

A Boolean value that indicates whether a request is in process.

