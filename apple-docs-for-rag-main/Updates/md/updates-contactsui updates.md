

- Updates
-  ContactsUI updates 

Article

# ContactsUI updates

Learn about important changes to ContactsUI.

## Overview

Browse notable changes in ContactsUI.

## June 2024

### Limited access to contacts

- Check your app’s authorization status for a new value, `CNAuthorizationStatus.limited`. This represents a new status in which a person can grant your app access to a limited subset of their contacts, rather than make an all-or-nothing choice. When your app first calls `CNContactStore.requestAccess(for:completionHandler:)`, an alert asks the person using the app whether to allow contacts access at all. If they allow access, they can choose either full access or choose which contacts to allow, which appears to your app as the `.limited` authorization status. They can revise their choices later in the Settings app.

- Allow someone to quickly add more contacts to this limited-access group by displaying a `ContactAccessButton` in your app’s contact search UI. You initialize this SwiftUI view with a search substring and sets of ignored emails and phone numbers. If a single person matches this query, the button shows the contact and offers to add them to the contacts your app can access. If there are multiple matches, tapping the button shows a separate view to select contacts.

- Use the SwiftUI view modifier `contactAccessPicker(isPresented:completionHandler:)` if you want to conditionally show a full-screen picker that adds contacts to your limited-access app. The `isPresented` parameter binds to a `Bool` value, and shows the picker when the bound value becomes `true`.

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

App Intents updates

Learn about important changes in App Intents.

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

Core Location updates

Learn about important changes to Core Location.

