

- ImageCaptureCore
- ICDeviceBrowser
-  resetControlAuthorization(completion:) 

Instance Method

# resetControlAuthorization(completion:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
func resetControlAuthorization(completion: @escaping (ICAuthorizationStatus) -> Void)
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

func resetControlAuthorization() async -> ICAuthorizationStatus

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

