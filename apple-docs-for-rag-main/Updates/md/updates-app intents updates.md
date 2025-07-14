

- Updates
-  App Intents updates 

Article

# App Intents updates

Learn about important changes in App Intents.

## Overview

Browse notable changes in App Intents.

## November 2024

### Siri and Apple Intelligence

- Make onscreen content available to Siri and Apple Intelligence by describing it as an AppEntity and adopting an assistant schema. Additionally, adopt the Transferable protocol, and associate the app entity with a NSUserActivity using the activity’s appEntityIdentifier property.

## June 2024

### System integration

- Integrate your app with Siri and Apple Intelligence using App intent domains.

- Use ControlConfigurationIntent and WidgetKit to allow users to put controls on the Lock Screen or in Control Center.

- Create a locked camera capture extension for your app and implement a CameraCaptureIntent to allow people to capture photos and videos from controls or the Action button.

- Create app intents that capture audio by implementing AudioRecordingIntent.

- Allow people to find app entities in Spotlight by adopting the IndexedEntity protocol.

### Content sharing

- Make it possible to share and transfer data you describe as App entities by conforming to Transferable.

- Receive content other apps make available with app intents by using IntentFile for your app intent parameters.

- Describe the file that stores your app intent data using FileEntity.

### General

- Provide additional information about errors with AppIntentError.PermissionRequired, AppIntentError.Unrecoverable, and AppIntentError.UserActionRequired.

- Pass a condition to requestConfirmation(conditions:actionName:dialog:) to only require user confirmation if a person’s context meets the provided condition.

- Use URLRepresentableIntent, URLRepresentableEntity, and URLRepresentableEnum to represent your app intents, app entities, and app enums as universal links that you use to provide deep links to your app’s content.

- Define a set of types for an intent parameter using the UnionValue() macro to create flexible app intents because a parameter can be of one of several pre-defined union types.

- Create entities that have just one singular instance with UniqueAppEntity and the corresponding UniqueAppEntityQuery. For example, to provide an app intent for app settings that appear in your app or in System Settings, create a singleton entity that encapsulates all settings as properties. Use it in the app intent that offers actions to change your app’s settings.

## See Also

### Technology updates

Accelerate updates

Learn about important changes to Accelerate.

Accessibility updates

Learn about important changes to Accessibility.

ActivityKit updates

Learn about important changes in ActivityKit.

AdAttributionKit Updates

Learn about important changes to AdAttributionKit.

AppKit updates

Learn about important changes to AppKit.

Apple Intelligence updates

Learn about important changes to Apple Intelligence.

Apple Pencil updates

Learn about important changes to Apple Pencil.

ARKit updates

Learn about important changes to ARKit.

Audio Toolbox updates

Learn about important changes to Audio Toolbox.

AuthenticationServices updates

Learn about important changes to AuthenticationServices.

AVFAudio updates

Learn about important changes to AVFAudio.

AVFoundation updates

Learn about important changes to AVFoundation.

Bundle Resources updates

Learn about important changes to Bundle Resources.

ContactsUI updates

Learn about important changes to ContactsUI.

Core Location updates

Learn about important changes to Core Location.

