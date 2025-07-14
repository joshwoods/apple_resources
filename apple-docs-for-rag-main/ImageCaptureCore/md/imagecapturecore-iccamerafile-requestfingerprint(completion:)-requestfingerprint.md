

- ImageCaptureCore
- ICCameraFile
-  requestFingerprint(completion:) 

Instance Method

# requestFingerprint(completion:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
func requestFingerprint(completion: @escaping (String?, (any Error)?) -> Void)
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

func requestFingerprint() async throws -> String

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

