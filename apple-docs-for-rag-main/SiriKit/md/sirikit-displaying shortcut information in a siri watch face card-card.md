

- SiriKit
-  Displaying Shortcut Information in a Siri Watch Face Card 

Article

# Displaying Shortcut Information in a Siri Watch Face Card

Display and customize watch-specific shortcut information with a default card template.

## Overview

The Siri watch face displays a relevant shortcut in a card that can provide the following information:

- App icon and name (supplied by the system)

- Title, subtitle, and custom image (supplied by the intent or user activity used to create the shortcut, or by an INDefaultCardTemplate object)

### Display Intent-Based Shortcuts

When your app uses an INIntent object to create the shortcut, the system retrieves the intent’s title and subtitle from the intent settings defined in the intent definition file. To include an image, call setImage:forParameterNamed: on the intent and pass in an INImage.

The listing below sets the image for a order soup intent in the Soup Chef sample app.

```
orderSoupIntent.setImage(INImage(named: menuItem.iconImageName), forParameterNamed: \OrderSoupIntent.soup)
```

### Display User Activity-Based Shortcuts

When your app uses an NSUserActivity object to create the shortcut, the system retrieves the title from the title property of the user activity. To specify a subtitle, create an CSSearchableItemAttributeSet with the content type of `kUTTypeItem`, and set the contentDescription property. To include an image, set the thumbnailData on the attribute set.

The listing below sets the title, subtitle, and image for the NSUserActivity object.

```
import CoreSpotlight
import MobileCoreServices

let userActivity = NSUserActivity(activityType: "com.myapp.myactivity")
userActivity.title = "Title"

let attributes = CSSearchableItemAttributeSet(itemContentType: kUTTypeItem as String)
attributes.contentDescription = "Subtitle"
attributes.thumbnailData =  imageLiteral(resourceName: "custom-image").pngData()

userActivity.contentAttributeSet = attributes
```

### Use Card Templates

If you want to show a UI specific to the watch—for example, to display a shortcut’s title that is shorter than the one Siri displays on the user’s iPhone or iPad—provide the relevant shortcut a default card template by setting the watchTemplate property. The template allows your app to customize the title, subtitle, and image. (You cannot change or remove the app icon and name shown in the card.)

The listing below sets the template for an order intent in the Soup Chef sample app.

```
let order = Order(quantity: 1, menuItem: menuItem, menuItemOptions: [])
let orderIntent = order.intent

guard let shortcut = INShortcut(intent: orderIntent) else { return nil }

let suggestedShortcut = INRelevantShortcut(shortcut: shortcut)

let localizedTitle = NSString.deferredLocalizedIntentsString(with: "ORDER_LUNCH_TITLE") as String
let template = INDefaultCardTemplate(title: localizedTitle)
template.subtitle = NSString.deferredLocalizedIntentsString(with: menuItem.shortcutNameKey + "_SUBTITLE") as String
template.image = INImage(named: menuItem.iconImageName)

suggestedShortcut.watchTemplate = template
```

The code above creates the Siri watch face card shown in the figure below. To download the complete sample code, see doc://com.apple.documentation/documentation/sirikit/soup_chef_accelerating_app_interactions_with_shortcuts.

The system displays the information in one of four layouts based on the information your app provides in the card template. For instance, if you don’t provide an image, the system uses a layout that displays only the title and subtitle fields. And if you provide only the title, the system uses a layout that can wrap the title on two lines.

## See Also

### Related Documentation

Soup Chef: Accelerating App Interactions with Shortcuts

Make it easy for people to use Siri with your app by providing shortcuts to your app’s actions.

### Articles

Adding User Interactivity with Siri Shortcuts and the Shortcuts App

Add custom intents and parameters to help users interact more quickly and effectively with Siri and the Shortcuts app.

Defining Relevant Shortcuts for the Siri Watch Face

Inform Siri when your app’s shortcuts may be useful to the user.

Deleting Donated Shortcuts

Remove your donations from Siri.

Dispatching intents to handlers

Provide SiriKit with an intent handler capable of handling a specific intent.

Improving Siri Media Interactions and App Selection

Fine-tune voice controls and improve Siri Suggestions by sharing app capabilities, customized names, and listening habits with the system.

Improving interactions between Siri and your messaging app

Donate app-specific content, use Siri’s contact suggestions, and adopt the latest platform features to create a more consistent messaging experience.

Registering Custom Vocabulary with SiriKit

Register your app’s custom terminology, and provide sample phrases for how to use your app with Siri.

Confirming the Details of an Intent

Perform final validation of the intent parameters and verify that your services are ready to fulfill the intent.

Handling an Intent

Fulfill the intent and provide feedback to SiriKit about what you did.

Resolving the Parameters of an Intent

Validate the parameters of an intent and make sure that you have the information you need to continue.

Generating a List of Ride Options

Generate ride options for Maps to display to the user.

Handling the Ride-Booking Intents

Support the different intent-handling sequences for booking rides with Shortcuts or Maps.

Donating Reservations

Inform Siri of reservations made from your app.

Defining Relevant Shortcuts for the Siri Watch Face

Inform Siri when your app’s shortcuts may be useful to the user.

Specifying Synonyms for Your App Name

Provide alternative names for your app that are more familiar or easier for users to speak.

