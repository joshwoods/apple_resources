

- ImageCaptureCore
- ICCameraFile
-  requestSecurityScopedURL(completion:) 

Instance Method

# requestSecurityScopedURL(completion:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
func requestSecurityScopedURL(completion: @escaping (URL?, (any Error)?) -> Void)
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

func requestSecurityScopedURL() async throws -> URL

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

