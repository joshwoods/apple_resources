

- Media Player
- MPPlayableContentDelegate
-  playableContentManager(\_:initiatePlaybackOfContentItemAt:completionHandler:) Deprecated

Instance Method

# playableContentManager(\_:initiatePlaybackOfContentItemAt:completionHandler:)

Asks the delegate to begin playback of the specified content item.

iOS 7.1–14.0DeprecatediPadOS 7.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func playableContentManager(
    _ contentManager: MPPlayableContentManager,
    initiatePlaybackOfContentItemAt indexPath: IndexPath,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
optional func playableContentManager(
    _ contentManager: MPPlayableContentManager,
    initiatePlaybackOfContentItemAt indexPath: IndexPath
) async throws
```

Deprecated

Use CarPlay framework

## Parameters 

`contentManager`  

The content manager that initiated the request.

`indexPath`  

The index for the indicated item.

`completionHandler`  

A block that the system calls after initiating a playback request. The block takes the following parameter:

error  
Pass nil if playback successfully began. If playback can’t begin, pass an error to indicate the reason.

## Discussion

The system calls this method when a media player interface needs to play a media item. Your app responds by beginning playback of the requested media item. After beginning playback, call the provided `completionHandler` block with an argument of `nil`; or, if your app can’t begin playback, call the completion handler with an error that indicates the reason.

Important

Don’t automatically restart playback when the media item is already playing. In most cases, it’s better for your app to do nothing and continue to play the current media item.

