

- Media Player
-  Handling external player events notifications 

Article

# Handling external player events notifications

Handle events for external media players.

## Overview

Apps that play audio or video content receive player events to start and stop playback, change tracks, and even rate an item. All iOS apps that create their own media player, macOS apps, and external media apps should support these events.

Note

When you use either the system or application player, you don’t get event notifications because those players automatically handle events.

To receive player event notifications, do the following:

- Use the shared MPRemoteCommandCenter object to register handlers for the events you wish to handle and to disable the events you’re not interested to receive.

- Begin playing your content. Your app must be the Now Playing app. An app doesn’t receive remote control events until it begins playing content. Test that your app is properly receiving and handling remote control events with Control Center, which you access by swiping up from the bottom edge of your screen. These controls send remote control events to the app that’s currently or was most recently playing. You can also access the playback controls from the lock screen of the device.

You can ensure that your app interacts well with other apps handling remote control events by following the best practices laid out in the Becoming a now playable app sample code project.

## See Also

### External player and system event handling

Remote command center events

Set up the remote command center to handle media player events.

Track navigation events

Respond to requests to change which part of a media item plays.

Media playback mode events

Respond to changes in the way media items play.

Feedback and rating events

Respond to incoming feedback and rating events.

