

- ImageCaptureCore
- ICCameraFile
-  requestThumbnailData(options:completion:) 

Instance Method

# requestThumbnailData(options:completion:)

Requests a thumbnail and executes the completion block in place of the delegate.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func requestThumbnailData(
    options: [ICCameraItemThumbnailOption : Any]? = nil,
    completion: @escaping (Data?, (any Error)?) -> Void
)
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

func requestThumbnailData(options: [ICCameraItemThumbnailOption : Any]? = nil) async throws -> Data

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The completion block executes on an any available queue; often this is not the main queue.

