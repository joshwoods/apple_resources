

- Foundation
-  NSUserActivityTypeBrowsingWeb 

Global Variable

# NSUserActivityTypeBrowsingWeb

An activity that continues from Handoff or a universal link.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSUserActivityTypeBrowsingWeb: String
```

## Discussion

An NSUserActivity object with an activityType value of NSUserActivityTypeBrowsingWeb indicates either an activity continued from a web browser-to-native app Handoff or a universal link. For this activity type, the webpageURL property contains the `http` or `https` URL associated with the activity.

For more information on universal links, see Allowing apps and websites to link to your content. For more information on web browser-to-native app Handoff, see Web Browser–to–Native App Handoff.

## See Also

### Identifying activity types

let TVUserActivityTypeBrowsingChannelGuide: String

An activity for viewing your app’s channel guide.

