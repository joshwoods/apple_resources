

- WebKit
- WKWebView
-  setAllMediaPlaybackSuspended(\_:completionHandler:) 

Instance Method

# setAllMediaPlaybackSuspended(\_:completionHandler:)

Changes whether the webpage is suspending playback of all media in the page.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor
func setAllMediaPlaybackSuspended(
    _ suspended: Bool,
    completionHandler: (@MainActor () -> Void)? = nil
)
```

``` source
@MainActor
func setAllMediaPlaybackSuspended(_ suspended: Bool) async
```

## Parameters 

`suspended`  

A Boolean value that indicates whether the webpage should suspend media playback.

`completionHandler`  

A closure the system executes after it completes changing the media playback suspension status.

## Discussion

Pass `true` to pause all media the web view is playing. Neither the user nor the webpage can resume playback until you call this method again with `false`.

## See Also

### Interacting with media

func pauseAllMediaPlayback(completionHandler: (() -> Void)?)

Pauses playback of all media in the web view.

func requestMediaPlaybackState(completionHandler: (WKMediaPlaybackState) -> Void)

Requests the playback status of media in the web view.

func closeAllMediaPresentations(completionHandler: (() -> Void)?)

Closes all media the web view is presenting, including picture-in-picture video and fullscreen video.

enum WKMediaPlaybackState

An enumeration that describes whether an audio or video presentation is playing, paused, or suspended.

