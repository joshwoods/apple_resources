

- ActivityKit
-  Adding accessible descriptions to widgets and Live Activities 

Article

# Adding accessible descriptions to widgets and Live Activities

Describe the interface elements of your widgets and Live Activities to help people understand what they represent.

## Overview

Designing with accessibility in mind is a foundational principle when creating an app. It also applies to widgets and Live Activities. To allow people to customize how they interact with your widget or Live Activity, to verify VoiceOver works correctly for them, and to help people understand what each interface element represents, add accessibility labels to the SwiftUI views you create for each widget and Live Activity presentation.

### Provide accessibility labels

Add accessibility labels for each SwiftUI view you use as needed and make sure your accessibility labels fit the widget or Live Activity content. To review API that allows you to add accessible descriptions to SwiftUI views, see Accessible descriptions.

The example below shows how the Emoji Rangers: Supporting Live Activities, interactivity, and animations app uses the accessibilityLabel(_:) modifier to add an accessibility labels for minimal, compact leading, and compact trailing presentations.

```
import SwiftUI
import WidgetKit

struct AdventureActivityConfiguration: Widget {
    var body: some WidgetConfiguration {
        ActivityConfiguration(for: AdventureAttributes.self) { context in
            // Create the presentation that appears on the Lock Screen and as a
            // banner on the Home Screen of devices that don't support the
            // Dynamic Island.
            // ...
        } dynamicIsland: { context in
            // Create the presentations that appear in the Dynamic Island.
            DynamicIsland {
                // Create the expanded presentation.
                // ...
            } compactLeading: {
                // Create the compact leading presentation.
                Avatar(hero: context.attributes.hero, includeBackground: true)
                    .accessibilityLabel("The avatar of \(context.attributes.hero.name).")
            } compactTrailing: {
                // Create the compact trailing presentation.
                ProgressView(value: context.state.currentHealthLevel, total: 1) {
                    let healthLevel = Int(context.state.currentHealthLevel * 100)
                    Text("\(healthLevel)")
                        .accessibilityLabel("Health level at \(healthLevel) percent.")
                }
                .progressViewStyle(.circular)
                .tint(context.state.currentHealthLevel 

If you provide a content description for an image you update while a Live Activity is active and the image conveys status information or similar, make sure to also update the accessibility label to match the updated status. For example, if an image indicates a delivery status, make sure the accessibility label changes as the delivery status that the image indicates changes. Similarly, update accessibility labels when a widget updates displayed images or SwiftUI views. For guidance on providing content descriptions, see Human Interface Guidelines > Accessibility > VoiceOver > Content descriptions.

## See Also

### Live Activity implementation

Displaying live data with Live Activities

Display your app’s data in the Dynamic Island and on the Lock Screen and offer quick interactions.

Starting and updating Live Activities with ActivityKit push notifications

Use ActivityKit to receive push tokens and to remotely start, update, and end your Live Activity with ActivityKit notifications.

class Activity

The object you use to start, update, and end a Live Activity.

Emoji Rangers: Supporting Live Activities, interactivity, and animations

Offer Live Activities, controls, animate data updates, and add interactivity to widgets.

NSSupportsLiveActivities

A Boolean value that indicates whether an app supports Live Activities.

NSSupportsLiveActivitiesFrequentUpdates

A Boolean value that indicates whether an app can update its Live Activities frequently.

