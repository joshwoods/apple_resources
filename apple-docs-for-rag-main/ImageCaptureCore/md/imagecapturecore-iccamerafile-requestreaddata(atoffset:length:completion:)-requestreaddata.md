

- ImageCaptureCore
- ICCameraFile
-  requestReadData(atOffset:length:completion:) 

Instance Method

# requestReadData(atOffset:length:completion:)

Requests to asynchronously read data of a specified length from a specified offset, then executes the completion block.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func requestReadData(
    atOffset offset: off_t,
    length: off_t,
    completion: @escaping (Data?, (any Error)?) -> Void
)
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

func requestReadData(atOffset offset: off_t, length: off_t) async throws -> Data

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The completion block executes on an any available queue; often this is not the main queue.

