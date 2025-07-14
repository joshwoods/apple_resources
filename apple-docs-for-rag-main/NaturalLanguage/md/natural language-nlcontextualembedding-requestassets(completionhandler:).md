

- Natural Language
- NLContextualEmbedding
-  requestAssets(completionHandler:) 

Instance Method

# requestAssets(completionHandler:)

Requests assets for an embedding, if available.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func requestAssets(completionHandler: @escaping (NLContextualEmbedding.AssetsResult, (any Error)?) -> Void)
```

``` source
func requestAssets() async throws -> NLContextualEmbedding.AssetsResult
```

## Parameters 

`completionHandler`  

A completion handler the system calls after it finishes the request.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func requestAssets() async throws -> NLContextualEmbedding.AssetsResult
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

You use a contextual embedding after loading the necessary assets onto the device. Use hasAvailableAssets to determine whether assets are available.

This method returns immediately if the framework knows the state of the assets or if an error occurs.

## See Also

### Requesting assets

enum AssetsResult

The status of an asset request.

