

- Group Activities
- GroupSessionEvent
-  url 

Instance Property

# url

The URL to open when the participant taps the event link in the system UI.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
let url: URL?
```

## Discussion

When the user taps your custom event in the system UI, the system opens the provided URL. Specify a universal link to open your app to the place where the action occurred. If the value of this link is `nil`, the system brings your app to the foreground.

For information about how to support universal links in your app, see Supporting universal links in your app

## See Also

### Getting the event details

let originator: Participant

The participant that initiated the event.

let action: GroupSessionEvent.Action

The reason for the event.

struct Action

A playback-related change that occurs during the session.

