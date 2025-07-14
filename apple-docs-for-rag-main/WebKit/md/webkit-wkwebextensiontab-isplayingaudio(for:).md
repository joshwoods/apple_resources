

- WebKit
- WKWebExtensionTab
-  isPlayingAudio(for:) 

Instance Method

# isPlayingAudio(for:)

Called to check if the tab is currently playing audio.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func isPlayingAudio(for context: WKWebExtensionContext) -> Bool
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

Defaults to `NO` if not implemented.

