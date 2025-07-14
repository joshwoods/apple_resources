

- WidgetKit
-  Developing a WidgetKit strategy 

Article

# Developing a WidgetKit strategy

Explore features, tasks, related frameworks, and constraints as you make a plan to implement widgets, watch complications, and Live Activities.

## Overview

Use WidgetKit to build widgets, watch complications, and Live Activities. With these features, you can create an ecosystem across platforms and devices, expanding the reach of your app. Widgets, complications, and Live Activities use WidgetKit and a set of related frameworks, including SwiftUI and App Intents, to take up limited but effective, eye-catching space. Because their design, functionality, and code are similar, they’re perfect candidates for code and design component reuse.

To avoid costly changes in your app’s development process, plan your WidgetKit adoption before you create designs and write code. As you make your plans, take into account:

- Feature availability for each platform

- Frameworks to use in addition to WidgetKit

- Required appearances and available sizes for widgets, watch complications, and Live Activities

- Technology that powers content updates

- Animation

- Interactivity with your app through deep links, buttons, and toggles

- Configuration options for widgets and watch complications

- Visibility in Smart Stacks

- Functional constraints

### Offer glanceable experiences in various sizes and across platforms

Widgets come in many different sizes, from circular accessory widgets on the Lock Screen and complications on Apple Watch to extra-large widgets on iPad and Mac. It’s up to you to choose the sizes and complications you want to support, but consider supporting as many sizes and complications as possible.

This table shows the functionality available for each platform:

| Widget size or technology | iPhone | iPad | Apple Watch | Mac |
|----|----|----|----|----|
| Small system widgets | Home Screen, Today View, and StandBy | Home Screen, Today View, and Lock Screen | No | Yes |
| Medium system widgets | Home Screen and Today View | Home Screen and Today View | No | Yes |
| Large system widgets | Home Screen and Today View | Home Screen and Today View | No | Yes |
| Extra large system widgets | No | Home Screen and Today View | No | Yes |
| Circular accessory widgets | Lock Screen | Lock Screen | Watch complications and Smart Stack | No |
| Corner accessory widgets | No | No | Watch complications | No |
| Rectangular accessory widgets | Lock Screen | Lock Screen | Watch complications and Smart Stack | No |
| Inline accessory widgets | Lock Screen | Lock Screen | Watch complications | No |
| Live Activities | Yes | Yes | No | No |

Live Activities are available on iPhone and iPad and appear on the Lock Screen. On devices that support the Dynamic Island, Live Activities appear in the Dynamic Island in compact, minimal, and extended appearances. On devices that don’t support the Dynamic Island, Live Activities appear briefly on the Home Screen, and as an overlay in other apps to notify people of updated data if you choose to alert people about the update.

Important

You need to support all Live Activity appearances, from minimal and compact presentations to larger extended and Lock Screen presentations.

Approach WidgetKit adoption iteratively. For example, start with a nonconfigurable WidgetFamily.systemSmall widget as described in Creating a widget extension because it gives your content broad exposure in the WidgetKit ecosystem on iPhone, iPad, and Mac. Then, add support for configuration, additional widget sizes, and — depending on your app’s features — Live Activities or a watchOS app with watch complications.

### Leverage additional frameworks

Widgets, watch complications, and Live Activities use a widget extension you add to your Xcode project. The role of WidgetKit is to provide the infrastructure and configuration for the features it enables. Depending on features and platforms you support, you use WidgetKit in combination with other frameworks as follows:

- To create the user interface for each feature, use SwiftUI.

- To add interactivity to widgets and Live Activities, use SwiftUI and the App Intents framework.

- To offer watch complications, create a watchOS app.

- To make widgets configurable, to offer preconfigured watch complications, and to enable functionalities like Smart Stacks and Widget Suggestions, use App Intents and SiriKit intents.

- To start, update, and end Live Activities, use ActivityKit.

### Support different appearances

Depending on the context, a widget or Live Activity changes its appearance to best fit its context. For example, a WidgetFamily.systemSmall widget appears as follows:

- On the Home Screen of iPhone and iPad, it uses the fullColor or accented rendering modes for light and dark appearances.

- On the Lock Screen of iPad and iPhone, it uses the vibrant rendering mode that provides a vibrant, blurred appearance. On the Lock Screen of iPhone in StandBy and StandBy in Night Mode, it renders scaled up in size using the vibrant rendering mode.

- On Mac, it uses the fullColor rendering mode in Notification Center for light and dark appearances. On the desktop, the widget appears receded with the vibrant appearance and changes to the fullColor appearance when a person interacts with it.

Similarly, the WidgetFamily.accessoryRectangular widget appears as follows:

- On the Lock Screen of iPhone and iPad, it takes on the vibrant appearance.

- On Apple Watch, it appears as a watch complication without a background and the accented appearance and in a fullColor appearance in the Smart Stack.

With each feature you add to your app, make sure your widget, watch complication, or Live Activity supports all applicable contexts and appearances well.

For more information, see Preparing widgets for additional platforms, contexts, and appearances.

For design guidance, see Human Interface Guidelines > Widgets.

### Animate content updates

On devices that run iOS 16, macOS 13, or earlier, widgets don’t use animations. However, Live Activities use the system’s animation timing to animate dynamic content and the addition or removal of views. For example, you can use built-in transitions for content or state changes, such as move(edge:).

Starting with iOS 17 and macOS 14, widgets can use animations, and both widgets and Live Activities can use custom animations. For more information, see Animating data updates in widgets and Live Activities.

### Provide up-to-date information with a timeline

Widgets and watch complications use a mechanism to update their content that’s different from your app. They use a timeline of data updates that you create in your app and hand to WidgetKit. You maintain this timeline as your app receives new data, but, to optimize battery life for a device, each app has a budget to update its widgets or complications. Additionally, the system batches and schedules updates to preserve power. For more information on how timelines work and how you can keep your widgets and watch complications up to date, see Keeping a widget up to date and Making network requests in a widget extension.

Live Activities don’t use timelines to update their content. Instead, they use ActivityKit and the Apple Push Notification service (APNs) to send ActivityKit push notifications. For more information, see ActivityKit.

### Add specific app functionality to your widgets and Live Activities

By default, people tap a widget, watch complication, or Live Activity to launch its corresponding app. To make the experience more intuitive and require fewer interactions, you can use deep linking to launch the scene of your app that matches the widget’s visible content. Widgets that offer enough space, such as WidgetFamily.systemSmall or larger — and Live Activities in the extended or the Lock Screen appearance — add SwiftUI’s Link to your views and allow people to open different screens in your app.

Note

In iOS 16 and macOS 13 or earlier versions, only large and extra-large widgets can use Link.

Starting with iOS 17 and macOS 14, widgets offer direct interaction with your app using the App Intents framework and SwiftUI. Both Button and Toggle offer dedicated initializers for this purpose. For more information, see Adding interactivity to widgets and Live Activities.

### Offer configurable widgets and watch complications

Make it possible for people to select the information they want to view in the widget by offering configurable iOS and macOS widgets that provide customizable properties. For example, people might choose to stay informed about a specific stock in a stock market widget, or enter a tracking number for a package delivery widget. Configurable widgets use the App Intents framework and custom intents you define — the same mechanism you use to support system-level services like Siri and the Shortcuts app. For information about creating a configurable widgets, see Making a configurable widget.

On Apple Watch, offer preconfigured watch complications to people with WidgetKit and the App Intents framework.

### Increase visibility in Smart Stacks

On iPhone and iPad, people create stacks of widgets, swipe through them manually, and use Smart Rotate to create Smart Stacks. In a Smart Stack, WidgetKit shows the widget at the top of a stack that matches a person’s context. For example, a weather widget might appear on the top of a Smart Stack each time a person leaves their home. To make sure the system shows your widget at the top of a Smart Stack at the right moment, use the App Intents framework.

On Apple Watch, the Smart Stack displays a list of default widgets and widgets a person adds to it. Like on iPhone and iPad, you use the App Intents framework to make sure people can add your widget to the Smart Stack.

For more information, see Increasing the visibility of widgets in Smart Stacks.

### Consider user privacy

The Lock Screen and watch faces are always visible, and people can configure widgets and complications to hide sensitive information when the device is locked or supports Always On. Review data that appears on your widget, Live Activity, or complication, and make sure you support redaction of sensitive data. For additional information, refer to Creating a widget extension.

### Store shared data in a group container

To add widgets, watch complications, and Live Activities, you create a widget extension and add it to your app, and the extension target and your app are part of the same app group. As a result, you can store files and data in a shared container that’s accessible to the app and the widget extension. For example, your app can download data and store it in a database in the shared container, and then a widget can access the database.

For additional information about app groups and accessing a shared container, refer to Configuring app groups.

### Respect functional constraints

Widgets, watch complications, and Live Activities are always visible. To preserve battery life and user privacy, they follow certain constraints. For example, Live Activities can’t access a person’s location. The following table shows availability features that impact battery life or user privacy for each feature:

| Functionality   | Widgets | Watch complications | Live Activities |
|-----------------|---------|---------------------|-----------------|
| Network access  | Yes     | Yes                 | No              |
| Location access | Yes     | Yes                 | No              |

For additional information, see Accessing location information in widgets.

## See Also

### Essentials

WidgetKit updates

Learn about important changes in WidgetKit.

