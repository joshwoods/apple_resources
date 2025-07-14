

- ReplayKit
- RPScreenRecorder
-  exportClip(to:duration:completionHandler:) 

Instance Method

# exportClip(to:duration:completionHandler:)

Exports a clip recording to a file.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.2+visionOS 1.0+

``` source
func exportClip(
    to url: URL,
    duration: TimeInterval,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func exportClip(
    to url: URL,
    duration: TimeInterval
) async throws
```

## Parameters 

`url`  

The URL of the destination file.

`duration`  

The duration for clip recording, in seconds. The system caps the duration at to the elapsed time, or a maximum of 15 seconds, whichever is shorter.

`completionHandler`  

A closure the system calls after it finishes exporting the clip. The system passes an error object to the closure if it encountered a problem writing the clip to disk.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func exportClip(to url: URL, duration: TimeInterval) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Performing Clip Recording

func startClipBuffering(completionHandler: (((any Error)?) -> Void)?)

Starts buffering a clip recording.

func stopClipBuffering(completionHandler: (((any Error)?) -> Void)?)

Stops buffering a clip recording.

