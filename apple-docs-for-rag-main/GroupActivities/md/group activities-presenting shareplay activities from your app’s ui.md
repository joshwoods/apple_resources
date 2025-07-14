

- Group Activities
-  Presenting SharePlay activities from your app’s UI 

Article

# Presenting SharePlay activities from your app’s UI

Make it easy for people to start activities from your app’s UI, from the system share sheet, or using AirPlay over AirDrop.

## Overview

After you define one or more SharePlay activities for your app, make them easy for people to discover in your UI. Include buttons, menus items, and other elements to start activities, present activities in system interfaces like the share sheet, and update your activities to take advantage of other system behaviors.

Starting an activity requires an active FaceTime call or Messages conversation. When a conversation is active, you can start an activity right away from your UI. If no conversation is active, the Group Activities framework facilitates starting a conversation as part of starting your activity. Some system features also help you start conversations.

For guidance about the best ways to add SharePlay support to your app’s UI, see Human Interface Guidelines > SharePlay.

### Add a SharePlay button to your UI

The most direct way to start activities is to provide controls in your UI. Because you control the placement of buttons and other controls in your UI, you can put them where people are most likely to find them. Provide a label or additional context to let someone know that your UI element starts an activity. For example, update your button’s label to include the `shareplay` symbol from the SF Symbols library.

The following example shows a SwiftUI button with both a text label and the SharePlay icon:

```
Button {
    // Start the activity.
} label: {
    Label("Start Activity", systemImage: "shareplay")
}
.buttonStyle(.borderedProminent)
```

In iOS, the preceding example creates a button with a prominent appearance as shown below. When creating buttons in your app, use a style that makes sense for the current platform and your app’s design.

When someone interacts with your app’s custom buttons, start the corresponding activity immediately if there is an active FaceTime call or Messages conversation. To determine if a conversation is active, check the isEligibleForGroupSession property of GroupStateObserver. If the value of that property is true, call the prepareForActivation() or activate() method of your GroupActivity type to start the activity. If the value of the property is `false`, present a `GroupActivitySharingController`, which prompts the person to invite friends to join the activity.

### Share activities in SwiftUI using a share link

To surface SharePlay activities using the system share sheet in SwiftUI, configure a ShareLink view with items that have an associated activity. A ShareLink view adds a standard share button to your UI, and you can customize the appearance of that button using the buttonStyle(_:) modifier. Tapping or clicking the button displays the system share sheet for the provided items. A person can then use the sheet to copy the items to the pasteboard or send them to a different process.

To surface your SharePlay activities from a ShareLink view, include a representation that contains your GroupActivity type. The share sheet in SwiftUI requires items to support the Transferable protocol. Adopt this protocol in your custom data types and implement the transferRepresentation property. Use that property to supply the representations of your data, and add a GroupActivityTransferRepresentation type to specify the GroupActivity for that data.

The following example shows the implementation of a movie data type and its transferRepresentation property. The property returns two representations: one for the movie’s URL and one for the movie-watching activity. The closure for the GroupActivityTransferRepresentation creates the `WatchMovieTogether` activity and initializes it with the selected movie.

```
struct Movie : Transferable {
    var title : String
    var url: URL

    static var transferRepresentation: some TransferRepresentation {
        // Export the movie as a URL.
        ProxyRepresentation(exporting: \.url) 

        // Specify the associated SharePlay activity.
        GroupActivityTransferRepresentation { movie in
            WatchMovieTogether(from: movie)
        }
    }
}
```

The following example creates a ShareLink to share a movie associated with the current view. When someone displays the share sheet and clicks the SharePlay link, the system initializes the app’s `WatchMovieTogether` activity with the specified movie and starts the activity.

```
ShareLink(item: movie,
          preview: .init("Play the movie together"))
```

### Add activities to the system share sheet in UIKit or AppKit

When displaying a share sheet using UIKit or AppKit, specify any SharePlay activities using NSItemProvider objects. When you configure the UIKit or AppKit share sheets, you specify one or more NSItemProvider objects with the data you want to share. If you have an activity you want to share for that item, create an instance of the appropriate GroupActivity type and pass it to the item provider’s registerGroupActivity(_:) method. When an item provider has a registered activity, the share sheet displays a SharePlay button to start the associated activity.

The following example creates a `WatchMovieTogether` activity to allow friends to watch a movie over SharePlay. After it creates an item provider for the movie, it registers the activity with that item provider and displays the share sheet. When someone clicks the SharePlay button in the share sheet, the system starts the movie-watching activity.

```
let activity = WatchMovieTogether(movie: movie)

// Create an item provider for the activity.
if let itemProvider = NSItemProvider(contentsOf: movie.url) {
    itemProvider.registerGroupActivity(activity)

    // Create and present the share sheet.
    let shareSheet = UIActivityViewController(activityItems: [itemProvider], applicationActivities: nil)
    shareSheet.allowsProminentActivity = true

    present(shareSheet, animated: true)
}
```

In AppKit, display the share sheet using an NSSharingServicePicker object. When creating the picker object, specify your NSItemProvider objects as the items you want to share.

### Share activities using SharePlay over AirDrop

SharePlay over AirDrop lets one person initiate an activity on their iPhone and share that activity with people in close proximity. The initiator opens an app on their iPhone and navigates to a page with the activity they want to start. When their iPhone comes in close proximity to other people’s iPhone devices, the initiator’s phone prompts them to start the activity. After they start the activity, the system prompts the other people to join and creates a Messages conversation for the group. Anyone in the group can then invite others to join the conversation and activity, including people who aren’t nearby.

In a SwiftUI app, the system enables SharePlay over AirDrop when the UI contains a ShareLink with an appropriate activity. The activity you include in the link must adopt the Transferable protocol and provide a GroupActivityTransferRepresentation type in its set of representations.

To support SharePlay over AirDrop in a UIKit app, assign activities to objects in the responder chain of your app’s UI. Typically, you add activities to your app’s view controllers, but you can add activities to any responder. When devices are nearby, the system searches the responder chain for a responder that contains an activity in its activityItemsConfiguration property. If an activity is available, the system displays UI to start that activity on the initiator’s device. The activityItemsConfiguration property stores one or more NSItemProvider objects, which you configure with activities by calling the registerGroupActivity(_:) method.

### Display activities in the Share menu in visionOS

In a visionOS app, the system displays a Share menu above windows and volumes to indicate when sharing is active. The system populates this control with activities the current scene supports.

- Not sharing
- Select an activity
- Sharing started

The Share menu is in the idle state, and sharing is not active for the window.

The person chooses an activity from the Share menu.

The Share menu is in the active state, and an activity is in progress.

Specify activities in any of the following ways:

- Include a ShareLink view with a properly configured activity, as described in Share activities using SharePlay over AirDrop.

- Configure the activityItemsConfiguration property of a UIKit responder object with an activity object.

- Associate an activity with the scene. See Adding spatial Persona support to an activity.

## See Also

### Interface presentation

class GroupActivitySharingController

A macOS view controller that displays the system interface for starting an activity, and optionally starts a FaceTime call for that activity.

class GroupActivitySharingController

An iOS view controller that displays the system interface for starting an activity, and optionally starts a FaceTime call for that activity.

