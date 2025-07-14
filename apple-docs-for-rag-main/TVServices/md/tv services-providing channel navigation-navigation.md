

- TV Services
-  Providing Channel Navigation 

Article

# Providing Channel Navigation

Support browsing an electronic program guide (EPG) and changing channels with specialized remote buttons.

## Overview

Some Apple TV-compatible remotes provide buttons specifically for browsing live TV or other multichannel content. Support these buttons in your app so users can access your electronic program guide (EPG) quickly.

For EPG design guidance, see the Human Interface Guidelines on Live-Viewing Apps. For guidance on designing remote interactions, see Remote.

### Display a Channel Guide

Some remotes provide a dedicated button for displaying TV channel listings or a similar EPG. For example, if you have a function named `activateChannelGuide()` that displays your EPG, add logic to your app’s UIApplicationDelegate to call `activateChannelGuide()` when your app receives a TVUserActivityTypeBrowsingChannelGuide user activity:

```
func application(_ application: UIApplication, continue userActivity: NSUserActivity, restorationHandler: @escaping ([UIUserActivityRestoring]?) -> Void) -> Bool {
    if #available(tvOS 14.3, *) {
        if (userActivity.activityType == TVUserActivityTypeBrowsingChannelGuide) {
            activateChannelGuide()
            return true
        }
    }
    // Handle other NSUserActivity types if appropriate.
    return false
}
```

Add TVUserActivityTypeBrowsingChannelGuide to the `NSUserActivityTypes` key in your app’s `Info.plist` file to inform the system of your app’s ability to handle this type of user activity.

When the user presses the Guide button while your app is active, the system sends the TVUserActivityTypeBrowsingChannelGuide to your app. When the user presses the Guide button while an app that doesn’t support the guide activity is active, the system sends the guide activity to the default guide app. The system also sends the user activity to the default guide app when the user long-presses the Guide button.

### Navigate an EPG

For an EPG that spans multiple screens, help users scan listings quickly, then navigate to the content they want. Respond to a UIPress.PressType.pageUp or UIPress.PressType.pageDown button press by moving to the previous or next screen of content, similar to a large swipe gesture.

### Change the Channel

While your content plays, change the channel when your app receives UIPress.PressType.pageUp or UIPress.PressType.pageDown.

```
override func viewDidLoad() {    
    super.viewDidLoad()

    let pageUpRecognizer = UITapGestureRecognizer(target: self, action: #selector(ViewController.channelUp))
    pageUpRecognizer.allowedPressTypes = [UIPress.PressType.pageUp.rawValue as NSNumber]
    view.addGestureRecognizer(pageUpRecognizer)

    let pageDownRecognizer = UITapGestureRecognizer(target: self, action: #selector(ViewController.channelDown))
    pageDownRecognizer.allowedPressTypes = [UIPress.PressType.pageDown.rawValue as NSNumber]
    view.addGestureRecognizer(pageDownRecognizer)
}

```

## See Also

### Channel guide

let TVUserActivityTypeBrowsingChannelGuide: String

An activity for viewing your app’s channel guide.

