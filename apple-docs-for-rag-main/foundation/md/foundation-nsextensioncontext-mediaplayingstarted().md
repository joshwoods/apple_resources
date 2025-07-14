

- Foundation
- NSExtensionContext
-  mediaPlayingStarted() 

Instance Method

# mediaPlayingStarted()

Tells the system that the Notification Content app extension began playing a media file.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func mediaPlayingStarted()
```

## Discussion

In your Notification Content app extension code, call this method when you programmatically begin playing a media file. When called, the system updates the appearance of the media playback button displayed in the notification content extension’s interface. For more information about implementing a notification content extension, see UNNotificationContentExtension.

## See Also

### Controlling media playback in notification content extensions

func mediaPlayingPaused()

Tells the system that the Notification Content app extension stopped playing a media file.

