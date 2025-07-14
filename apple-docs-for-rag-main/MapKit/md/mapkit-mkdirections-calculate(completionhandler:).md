

- MapKit
- MKDirections
-  calculate(completionHandler:) 

Instance Method

# calculate(completionHandler:)

Begins calculating the requested route information asynchronously.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func calculate(completionHandler: @escaping MKDirections.DirectionsHandler)
```

``` source
func calculate() async throws -> MKDirections.Response
```

## Parameters 

`completionHandler`  

The block to execute when the directions are ready or when an error occurs. This parameter can’t be `nil`.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func calculate() async throws -> MKDirections.Response
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method initiates the request for directions and calls your completion handler block with the results. The method executes your completion handler on your app’s main thread. The implementation of your handler needs to check for errors and then incorporate the response data as appropriate.

If you call this method while a previous request is in process, this method calls your completion handler with an error. You can determine whether a request is in process by checking the value of the isCalculating property. You can also cancel a request as necessary.

## See Also

### Related Documentation

var isCalculating: Bool

A Boolean value that indicates whether a request is in process.

func cancel()

Cancels a pending request.

### Getting the directions

typealias DirectionsHandler

The block to use for processing the requested route information.

class Response

The route information that Apple servers return in response to your request for directions.

