

- WebKit
- WKWebView
-  pauseAllMediaPlayback(completionHandler:) 

Instance Method

# pauseAllMediaPlayback(completionHandler:)

Pauses playback of all media in the web view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor
func pauseAllMediaPlayback(completionHandler: (@MainActor () -> Void)? = nil)
```

``` source
@MainActor
func pauseAllMediaPlayback() async
```

## Parameters 

`completionHandler`  

A closure the system executes after the web view pauses media playback.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func pauseAllMediaPlayback() async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Interacting with media

func requestMediaPlaybackState(completionHandler: (WKMediaPlaybackState) -> Void)

Requests the playback status of media in the web view.

func setAllMediaPlaybackSuspended(Bool, completionHandler: (() -> Void)?)

Changes whether the webpage is suspending playback of all media in the page.

func closeAllMediaPresentations(completionHandler: (() -> Void)?)

Closes all media the web view is presenting, including picture-in-picture video and fullscreen video.

enum WKMediaPlaybackState

An enumeration that describes whether an audio or video presentation is playing, paused, or suspended.

