

- ReplayKit
- RPScreenRecorder
-  startClipBuffering(completionHandler:) 

Instance Method

# startClipBuffering(completionHandler:)

Starts buffering a clip recording.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.2+visionOS 1.0+

``` source
func startClipBuffering(completionHandler: (((any Error)?) -> Void)? = nil)
```

``` source
func startClipBuffering() async throws
```

## Parameters 

`completionHandler`  

The system invokes this closure when recording starts. The system passes an error object to the closure if it encountered a problem.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func startClipBuffering() async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Performing Clip Recording

func stopClipBuffering(completionHandler: (((any Error)?) -> Void)?)

Stops buffering a clip recording.

func exportClip(to: URL, duration: TimeInterval, completionHandler: (((any Error)?) -> Void)?)

Exports a clip recording to a file.

