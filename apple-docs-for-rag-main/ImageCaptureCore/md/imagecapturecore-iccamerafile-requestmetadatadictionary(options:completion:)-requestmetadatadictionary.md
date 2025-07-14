

- ImageCaptureCore
- ICCameraFile
-  requestMetadataDictionary(options:completion:) 

Instance Method

# requestMetadataDictionary(options:completion:)

Requests metadata and executes the completion block in place of the delegate.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func requestMetadataDictionary(
    options: [ICCameraItemMetadataOption : Any]? = nil,
    completion: @escaping ([AnyHashable : Any]?, (any Error)?) -> Void
)
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

func requestMetadataDictionary(options: [ICCameraItemMetadataOption : Any]? = nil) async throws -> [AnyHashable : Any]

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The completion block executes on an any available queue; often this is not the main queue.

