

- WebKit
- WKWebView
-  setMicrophoneCaptureState(\_:completionHandler:) 

Instance Method

# setMicrophoneCaptureState(\_:completionHandler:)

Changes whether the webpage is using the microphone to capture audio.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor
func setMicrophoneCaptureState(
    _ state: WKMediaCaptureState,
    completionHandler: (@MainActor () -> Void)? = nil
)
```

``` source
@MainActor
func setMicrophoneCaptureState(_ state: WKMediaCaptureState) async
```

## Parameters 

`state`  

An enumeration case that indicates whether the webpage should use the microphone to capture audio.

`completionHandler`  

A closure the system executes after changing whether the webpage is using the microphone to capture audio.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func setMicrophoneCaptureState(_ state: WKMediaCaptureState) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Managing the microphone and camera

var cameraCaptureState: WKMediaCaptureState

An enumeration case that indicates whether the webpage is using the camera to capture images or video.

var microphoneCaptureState: WKMediaCaptureState

An enumeration case that indicates whether the webpage is using the microphone to capture audio.

func setCameraCaptureState(WKMediaCaptureState, completionHandler: (() -> Void)?)

Changes whether the webpage is using the camera to capture images or video.

enum WKMediaCaptureState

An enumeration that describes whether a media device, like a camera or microphone, is currently capturing audio or video.

