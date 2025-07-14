

- Technotes
-  TN3130: Changes to EventKit in macOS Ventura 13 

Article

# TN3130: Changes to EventKit in macOS Ventura 13

Test your apps against EventKit API changes in macOS Ventura 13.

## Overview

In macOS Ventura 13, the EventKit framework has seen significant changes. This document highlights some of the notable changes. To learn about related changes in iOS 16, see TN3132: Changes to EventKit and EventKitUI in iOS 16.

For apps running on systems prior to macOS Ventura 13, the legacy behavior remains in place when using EventKit. When you run your app on macOS Ventura 13, and have built it with Xcode 14 and linked against the macOS 13 SDK, you may see behavior that you are unfamiliar with when using EventKit. To identify these changes in behavior, thoroughly test your app for each major OS version it supports. Confirm that your implementation of EventKit behaves as you expect in each OS version and update your code where needed. If you notice an unexpected behavior in EventKit, report it using Feedback Assistant.

## EKCalendar

The inherited initializer `init()` throws an exception when attempting to create a new calendar. Use init(for:eventStore:) instead.

```
let calendar = EKCalendar(for: .event, eventStore: eventStore)
```

In the legacy behavior, this inherited initializer returns an unusable `EKCalendar` object.

## EKCalendarItem

### Fetching recurence rules

The recurrenceRules property returns an empty array if the calendar item doesn’t have any recurrence rules.

In the legacy behavior, `recurrenceRules` returns `nil` if the calendar item doesn’t have any recurrence rules.

### Updating time zones

Changing the time zone of an event no longer changes the absolute time at which it occurs.

## EKEvent

### Creating events

The inherited initializer `init()` throws an exception when attempting to create a new event. Use init(eventStore:) to create new events.

In the legacy behavior, this inherited initializer returns an unusable `EKEvent` object.

### Event identifiers

The eventIdentifier property now returns identifiers in a new format. The previous identifier format will continue to work.

### End date of all-day events

The end date property of all-day events returns a time of `11:59:59 PM` on the last day of this event.

```
Event title: Marathon  
Start date: June 18, 2022 at 12:00:00 AM PDT
End date: June 18, 2022 at 11:59:59 PM PDT
```

In the legacy behavior, this property returns a time of `12:00:00 AM` on the day after the event.

```
Event title: Marathon  
Start date: June 18, 2022 at 12:00:00 AM PDT
End date: June 19, 2022 at 12:00:00 AM PDT
```

## EKEventStore

### Accessing sources

The sources property now contains delegate sources.

```
// Fetch all sources associated with the event store.
let sources = eventStore.sources

sources.forEach { source in
    // Let's check whether source is a delegate event source.
    let name = (source.isDelegate) ? "Delegate Source" : "Source"
    print("\(name): \(source.title)")
}
// Prints "Source: iCloud"
// Prints "Delegate Source: Calculus Office Hours"
```

### Fetching events

events(matching:) and enumerateEvents(matching:using:) no longer necessarily return events sorted by start date.

### Accessing calendar events

The calendarItem(withIdentifier:), calendarItems(withExternalIdentifier:), and event(withIdentifier:) methods may return different occurrences of an event or reminder with a given identifier in some cases. For instance, when the first occurrence of a recurring event was modified and the specified identifier refers to this occurrence. In this case, use the given identifier to fetch the unmodified version of the event’s first occurrence.

### Committing changes

When you call saveCalendar(_:commit:), removeCalendar(_:commit:), save(_:span:commit:), remove(_:span:commit:), save(_:commit:), or remove(_:commit:) methods with the `commit` parameter set to `true`, EKEventStore attempts to immediatedly save and commit your changes to the event store. If the commit fails, `EKEventStore` automatically rolls back all changes that been saved but aren’t yet committed to the event store.

In the legacy behavior, uncommitted objects remain saved in the event store.

## EKReminder

The inherited initializer `init()` throws an exception when attempting to create a new reminder. Use init(eventStore:) instead.

```
let reminder = EKReminder(eventStore: eventStore)
```

In the legacy behavior, this inherited initializer returns an unusable `EKReminder` object.

## EKSource

The isDelegate property indicates whether the source is an event source delegated to the user.

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

