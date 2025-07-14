

- WebKit
- WKWebView
-  setCameraCaptureState(\_:completionHandler:) 

Instance Method

# setCameraCaptureState(\_:completionHandler:)

Changes whether the webpage is using the camera to capture images or video.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor
func setCameraCaptureState(
    _ state: WKMediaCaptureState,
    completionHandler: (@MainActor () -> Void)? = nil
)
```

``` source
@MainActor
func setCameraCaptureState(_ state: WKMediaCaptureState) async
```

## Parameters 

`state`  

An enumeration case that indicates whether the webpage should use the camera to capture images or video.

`completionHandler`  

A closure the system executes after changing whether the webpage is using the camera to capture images or video.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func setCameraCaptureState(_ state: WKMediaCaptureState) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Managing the microphone and camera

var cameraCaptureState: WKMediaCaptureState

An enumeration case that indicates whether the webpage is using the camera to capture images or video.

var microphoneCaptureState: WKMediaCaptureState

An enumeration case that indicates whether the webpage is using the microphone to capture audio.

func setMicrophoneCaptureState(WKMediaCaptureState, completionHandler: (() -> Void)?)

Changes whether the webpage is using the microphone to capture audio.

enum WKMediaCaptureState

An enumeration that describes whether a media device, like a camera or microphone, is currently capturing audio or video.

