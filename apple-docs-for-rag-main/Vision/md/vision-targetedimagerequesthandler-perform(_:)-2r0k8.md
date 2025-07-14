

- Vision
- TargetedImageRequestHandler
-  perform(\_:) 

Instance Method

# perform(\_:)

Performs a framework request on the handler’s image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final func perform(_ request: T) async throws -> T.Result where T : TargetedRequest
```

## See Also

### Performing the request

func perform&lt;each T>(repeat each T) async throws -> (repeat (each T).Result)

Performs one or more framework requests on the handler’s image.

func performAll(some Collection&lt;any TargetedRequest>) -> some AsyncSequence&lt;VisionResult, Never> 

Schedules a collection of framework requests to perform on the handler’s image.

