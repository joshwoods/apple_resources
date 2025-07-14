

- Technotes
-  TN3153: Adopting API changes for EventKit in iOS 17, macOS 14, and watchOS 10 

Article

# TN3153: Adopting API changes for EventKit in iOS 17, macOS 14, and watchOS 10

Test your existing apps against EventKit API latest changes.

## Overview

Xcode 15 includes SDKs for iOS 17, macOS 14, and watchOS 10 that introduce notable changes in EventKit such as new access levels: the ability to add events using EventKitUI without requesting access to Calendar, write-only access, and full access. Apps that don’t request access to calendar data use EKEventEditViewController to present UI for editing an event, which the person using your app can save. See Accessing the Event Store for details. If the user grants your app write-only access, your app can create and write calendar events. However, your app can’t read or delete any events from the user’s calendars, including the ones it creates. If the user grants your app full access, your app can read, write, create, and delete calendar events as in iOS 16 and earlier, for example. To learn how to update your app to use these new features, see TN3152: Migrating to the latest Calendar access levels.

If you built your app with an older version of Xcode 15 such as Xcode 14.3.1 and linked it against older versions of the iOS, macOS, or watchOS SDK, and run it on iOS 17, macOS 14, or watchOS 10, you may see behavior that you are unfamiliar with when using EventKit or EventKitUI. For instance, your app may not be able to fetch events even if the user previously granted full access to the app on an earlier OS version.

This document describes how some of these changes may affect your app. To identify these changes in behavior, thoroughly test your app for each major OS version it supports. Confirm that your usage of EventKit or EventKitUI behaves as you expect in each OS version and update your code where needed. If you notice an unexpected behavior in these frameworks, report it using Feedback Assistant.

## Calendar usage description keys

The NSCalendarsUsageDescription and NSRemindersUsageDescription keys describe how your app intends to use the user’s calendar data or reminders, respectively. If your app runs on iOS 17, macOS 14, watchOS 10, or later and doesn’t include the new NSCalendarsWriteOnlyAccessUsageDescription or NSCalendarsFullAccessUsageDescription key, EventKit uses `NSCalendarsUsageDescription` as fallback. If your app doesn’t include the new NSRemindersFullAccessUsageDescription key, EventKit uses `NSRemindersUsageDescription` as fallback.

## Requesting permission from the user

If your app links against an SDK older than the iOS 17 SDK, macOS 14 SDK, or watchOS 10 SDK and hasn’t previously prompted the user for calendar access,

**On iOS and macOS** Calling requestAccess(to:completion:) or requestAccess(to:) with an entity type `event` prompts the user to grant write-only calendar access to your app. If the user allows write-only access to your app and your app used `requestAccess(to:completion:)`, the system calls the EKEventStoreRequestAccessCompletionHandler completion handler with its boolean parameter set to `true`.

```
let eventStore = EKEventStore()
eventStore.requestAccess(to: .event, completion: {(granted, error) in
    if granted {
      // Fetch latest events.
    }
})
```

If the app called `requestAccess(to:)`, the system asynchronously returns a boolean value set to `true`.

```
let eventStore = EKEventStore()
let response = try await eventStore.requestAccess(to: .event)
if response {
    // Fetch latest events.
}
```

If the user denies access, the completion handler receives a `false` parameter and `requestAccess(to:)` returns `false`.

**On watchOS** Calling these methods with an entity type `event` prompts the user to grant full calendar access to your app.

Note

If the user previously granted write-only access to the iOS companion app, calling requestAccess(to:completion:) or requestAccess(to:) for events in the watchOS app doesn’t prompt the user for access. The access level of the watchOS app matches its companion app, which is write-only.

## Authorization status

An app with write-only or full access to calendar events will see its authorization status as authorized. If the user previously granted calendar access (`authorized`) to your app, calling authorizationStatus(for:) with an entity type event returns `authorized`.

```
EKEventStore.authorizationStatus(for: .event) == .authorized
```

The iOS, macOS, and watchOS SDKs bundled in Xcode 15 provide different levels of access: writeOnly and fullAccess. In an app linked against an SDK older than the iOS 17 SDK, macOS 14 SDK, or watchOS 10 SDK, `writeOnly` and `fullAccess` both map to `authorized`.

If the user previously granted calendar access to your app on an earlier OS, your app will have write-only access.

Note

Implement the new APIs if you want to distinguish between the `writeOnly` and `fullAccess` access levels in your app.

## Existing apps with write-only calendar access

If the user granted write-only access to your app,

- The sources property returns a single virtual source.

- The delegateSources property returns an empty array.

- The defaultCalendarForNewEvents property returns a single virtual calendar. The calendars(for:) method on EKEventStore and EKSource returns the same virtual calendar.

An app with write-only access may later request full access. The first time your app calls the calendarItemWithIdentifier:,  
calendarItemsWithExternalIdentifier:, enumerateEvents(matching:using:), events(matching:), or event(withIdentifier:) instance methods, it implicitly prompts the user to upgrade the app to full access or keep it write-only access. If the user grants full access to the app, an EKEventStoreChanged notification is posted, these methods return some results, and the app has a full access authorization status. When your app receives the event store notification, refetch all calendar data that your app needs to refresh its views. These data are now visible to your app.

If the user denies access, these methods don’t return any results, and any further calls don’t prompt the user for access again. Your app still has write-only calendar access.

Note

If your app doesn’t call calendarItemWithIdentifier:, calendarItemsWithExternalIdentifier:, enumerateEvents(matching:using:), events(matching:), or event(withIdentifier:) to implicitly prompt the user for upgrade, the user would have to know to change the access level for the app in Settings \> Privacy & Security \> Calendars on their device.

## Revision History

- **2024-02-27** Made minor editorial changes.

- **2023-06-06** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

