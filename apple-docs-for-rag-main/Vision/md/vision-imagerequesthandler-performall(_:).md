

- Vision
- ImageRequestHandler
-  performAll(\_:) 

Instance Method

# performAll(\_:)

Schedules a collection of framework requests to perform on the handler’s image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final func performAll(_ requests: some Collection) -> some AsyncSequence
```

## Parameters 

`requests`  

A collection of requests to perform.

## Return Value

A sequence of requests results.

## Discussion

This function doesn’t wait for requests to complete before returning. You can receive request results from the `AsyncSequence` as they become available.

## See Also

### Performing the request

func perform&lt;each T>(repeat each T) async throws -> (repeat (each T).Result)

Performs one or more framework requests on the handler’s image.

func perform&lt;T>(T) async throws -> T.Result

Performs a framework request on the handler’s image.

