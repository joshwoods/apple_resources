

- ImageCaptureCore
- ICDeviceBrowser
-  requestContentsAuthorization(completion:) 

Instance Method

# requestContentsAuthorization(completion:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func requestContentsAuthorization(completion: @escaping (ICAuthorizationStatus) -> Void)
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

func requestContentsAuthorization() async -> ICAuthorizationStatus

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

