

- SiriKit
-  Requesting Authorization to Use Siri 

Article

# Requesting Authorization to Use Siri

Request permission from the user for Siri and Maps to communicate with your app or Intents app extension.

## Overview

Siri can’t interact with your app or app extension until the user grants permission. Maps only interacts with your app extension, but as with Siri, only after the user authorizes it to do so. Request authorization from your iOS app, whether you’re handling intents in an app extension or in your app. When the user approves an authorization request from your iOS app, this grants permission for your iOS app, its Intents app extension, and your watchOS app.

Note

You don’t need to request authorization if your app only supports actions in the Shortcuts app.

### Configure Your App Target

First, enable the Siri capability for your iOS app or WatchKit extension for authorization to succeed. For information about how to enable the Siri capability, see Creating an Intents App Extension.

Next, configure your `Info.plist` file. Include the NSSiriUsageDescription key in your iOS appʼs `Info.plist` file. The value for this key is a string that describes what information your app shares with SiriKit. For example, a workout app might set the value to the string *Workout information will be sent to Siri*. This key is a requirement.

### Request User Authorization

Call the requestSiriAuthorization(_:) class method of INPreferences at some point during your iOS app’s execution.

Your app’s authorization status is INSiriAuthorizationStatus.notDetermined until the user authorizes or denies access. When your app requests authorization and its status is undetermined, the system prompts the user to authorize your app. The alert includes the usage description string you provided in the NSSiriUsageDescription key of your app’s `Info.plist` file.

The user can approve or deny your app’s request for authorization, and can change your app’s authorization status later in the Settings app. The system remembers your app’s authorization status so that subsequent calls to the requestSiriAuthorization(_:) method don’t prompt the user again.

Note

Siri and Maps may assist in authorizing your app or Intents app extension when the user first tries to use an intent you support. Specifically, if the user interacts with your app or app extension and your app’s authorization status isn’t yet determined, Maps requests authorization automatically on your extension’s behalf.

## See Also

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

Displaying Shortcut Information in a Siri Watch Face Card

Display and customize watch-specific shortcut information with a default card template.

Donating Reservations

Inform Siri of reservations made from your app.

Defining Relevant Shortcuts for the Siri Watch Face

Inform Siri when your app’s shortcuts may be useful to the user.

