

- Technotes
-  TN3132: Changes to EventKit and EventKitUI in iOS 16 

Article

# TN3132: Changes to EventKit and EventKitUI in iOS 16

Test your apps against EventKit and EventKitUI API changes in iOS 16.

## Overview

The iOS 16 SDK introduces some changes to the EventKit and EventKitUI frameworks. This document highlights some of the major changes. To learn about related changes in macOS Ventura 13, see TN3130: Changes to EventKit in macOS Ventura 13.

For apps running on systems prior to iOS 16, built with Xcode 13 or earlier and linked against older versions of the iOS SDK, the legacy behavior remains in place when using these frameworks. When you run your app on iOS 16, and have built it with Xcode 14 and linked against the iOS 16 SDK, you may see behavior that you are unfamiliar with when using EventKit or EventKitUI. To identify these changes in behavior, thoroughly test your app on each major OS version it supports on real hardware. Confirm that your implementation of EventKit or EventKitUI behaves as you expect in each OS version and update your code where needed.  
If you notice an unexpected behavior in EventKit, report it using Feedback Assistant.

## EKCalendarChooser

Setting the selectedCalendars property of a calendar chooser view controller no longer calls the calendarChooserSelectionDidChange(_:) delegate method. `calendarChooserSelectionDidChange(_:)` is only called when the user selects a calendar in the view controller.

## EKEventStore

### Committing changes

When you call saveCalendar(_:commit:), removeCalendar(_:commit:), save(_:span:commit:), remove(_:span:commit:), save(_:commit:), or remove(_:commit:) methods with the `commit` parameter set to `true`, EKEventStore attempts to immediatedly save and commit your changes to the event store. If the commit fails, `EKEventStore` automatically rolls back all changes that have been saved but aren’t yet committed to the event store.

In the legacy behavior, objects remain saved but uncommitted in the event store when the commit failed.

### Fetching events

events(matching:) and enumerateEvents(matching:using:) now return events that have been saved but weren’t yet committed to the event store.

In the legacy behavior, `events(matching:)` and `enumerateEvents(matching:using:)` only return events that have been saved and committed to the event store.

### Recurring events

If you are saving a detached occurrence of a recurring event, and you specify futureEvents for the `span` parameter of the save(_:span:commit:) method, your changes apply to all future occurrences of the event.

In the legacy behavior, your changes only apply to this instance of the recurring event.

## Revision History

- **2022-08-16** First published.

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

