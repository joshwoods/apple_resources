

- EventKit
-  Managing Location-Based Reminders 

Sample Code

# Managing Location-Based Reminders

Add, fetch, complete, remove, and sort location-based reminders in your app.

Download

iOS 13.0+iPadOS 13.0+Xcode 12.0+

## Overview

With the Reminders app, users can create reminders with attachments, and alarms based on time and location. When Location Services is turned on, users receive location-based reminders when entering or leaving a specified geographic area or geofence. This sample demonstrates how to add, fetch, complete, remove, and sort location-based reminders.

### Provide a Purpose String

The sample first requests and receives authorization from the user before the app attempts to access their reminder data. It provides a purpose string or usage description that describes how the app intends to use the user’s reminder data. It then adds the NSRemindersUsageDescription key to the app’s `Info.plist`. The sample sets its value to a string that explains why the app needs access to reminder data. The system displays the string when prompting the user for authorization.

Important

This `NSRemindersUsageDescription` key is required for apps that access the user’s reminder data. Apps crash when the key is absent.

### Request Authorization

Set up your app to instantiate and use a single instance of EKEventStore that manages all reminder-related tasks. An `EKEventStore` object requires a significant amount of time to initialize and release. The user might add, remove, or update reminders while your app is running. Register for an EKEventStoreChanged notification to be notified about changes to the Calendar database. When you receive this notification, refresh all your reminder data. It’s possible that your current data is stale or invalid. For more information on change notification, see Updating with Notifications for details.

The user grants or denies permission when apps request access to their reminder data. Because the user can change the app’s authorization status later in the Settings app ( Settings \> Privacy \> Reminders) on their device, the sample calls `EKEventStore`’s authorizationStatus(for:) with a EKEntityType.reminder entity type before attempting to access their reminder data.

```
guard EKEventStore.authorizationStatus(for: .reminder) == .notDetermined else {
    // The user may have already granted, denied, or restricted access to Reminders.
    verifyAuthorizationStatus()
    return
}
```

If the authorization status is .notDetermined, create an instance of `EKEventStore`, then store a strong reference to it.

```
private var store = EKEventStore()
```

Next, call its requestAccess(to:completion:) method to prompt the user for access.

```
store.requestAccess(to: .reminder, completion: {(granted, error) in
    if granted { self.accessGranted() }
})
```

The system remembers the user’s answer, so that subsequent calls to `requestAccess(to:completion:)` don’t again prompt the user. For more information on user’s reminder data access, see Accessing the Event Store.

### Map Annotations

The sample app uses the current user location and location-specific data saved in the `MapData.plist` file to create annotations for the map. It defines a `MapData` data type to represent each point of interest. `MapData.plist` contains three `MapData` entries. To test reminders around other locations, duplicate and update a `MapData` entry in `MapData.plist` with other data as needed.

Important

Creating location-based reminders doesn’t require location services. The sample app uses location services to display the user’s current location on the map. As such, it includes and configures the NSLocationWhenInUseUsageDescription key in its `Info.plist`. This key is required for apps that access the user’s location services. For more information on user’s location services access, see Requesting Authorization for Location Services.

### Check for the Existence of a Default List

Creating a reminder requires a list, which is a calendar for these items. Use `EKEventStore`’s defaultCalendarForNewReminders() to check whether the user has specified a default list for reminders. If `defaultCalendarForNewReminders()` returns no value, prompt the user to create a list in the Reminders app or provide a mechanism that lets them create it from within the app. The app provides an `Add List` button that allows users to create a new list.

### Create Location-Based Reminders

A location-based reminder is a reminder created with a geofence-enabled alarm. A geofence-enabled alarm has a structured location and proximity configured. The structured location consists of a location object and radius. The radius is defined in meters and uses the system’s default radius when its value is 0. When the user provides a value for `radius` in a unit other than meters such as miles, convert this value before using it. The sample uses the following steps to create a location-based reminder.

First, it creates an EKReminder object using init(eventStore:), then it sets its title and calendar properties:

```
guard let calendar = store.defaultCalendarForNewReminders() else { throw LocationBasedRemindersError.missingDefaultRemindersList }
let reminder = EKReminder(eventStore: store)
reminder.calendar = calendar
reminder.title = title
```

Important

The `title` and `calendar` properties are required and must be set before saving the reminder.

Next, it creates a structured location by using either EKStructuredLocation’s init(title:) or init(mapItem:). When the location object has latitude and longitude coordinates, it uses `init(title:)` to create the structured location. The sample initializes an CLLocation object with the specified latitude and longitude, then assigns it to the created structured location’s geoLocation property:

```
let structuredLocation = EKStructuredLocation(title: geofence.title)
structuredLocation.geoLocation = CLLocation(latitude: coordinate.latitude, longitude: coordinate.longitude)
```

When the location object is an MKMapItem object, the sample uses `init(mapItem:)` to create the structured

```
let structuredLocation = EKStructuredLocation(mapItem: mapItem)
```

Then, it sets the structured location’s `radius` property to a value in meters:

```
// The app displays the radius's value in miles. Let's convert it from miles to meters before assigning it to the radius property.
structuredLocation.radius = 1609.344 * geofence.radius
```

After that, it creates an EKAlarm object, then sets its structuredLocation property to the created structured location object. The sample then sets the proximity property to a value to finish configuring the alarm’s geofence:

```
let alarm = EKAlarm()
alarm.structuredLocation = structuredLocation
alarm.proximity = geofence.proximity
```

The sample adds the created alarm to the reminder. For more information on adding alarms, see Setting an Alarm.

```
reminder.addAlarm(alarm)
```

Finally, it saves the reminder to the user’s Calendar database:

```
do {
    try store.save(reminder, commit: true)
} catch {
    handleError(error, with: reminder.title)
}
```

### Fetch Location-Based Reminders

The fetchReminders(matching:completion:) method asynchronously fetches all reminders matching a given predicate. When successful, `fetchReminders(matching:completion:)` returns an array that contains both time-based and location-based reminders.

```
// Predicate that fetches all reminders in all of the user's calendars.
let predicate = store.predicateForReminders(in: nil)
var result = [EKReminder]()
store.fetchReminders(matching: predicate, completion: {(reminders: [Any]?) in
    if let reminders = reminders as? [EKReminder] {
        // Filter reminders for the location ones.
        result = reminders.filter({ (item: EKReminder) in item.isLocation })
    }

    DispatchQueue.main.async {
        completion(result)
    }
})
```

To retrieve location-based reminders, the sample parses this array for reminders defined with an existing alarm that has a `structuredlocation` and `proximity` value.

```
/// Indicates whether a reminder is a location-based one.
var isLocation: Bool {
    guard let alarms = self.alarms else { return false }

    return !alarms.filter({(alarm: EKAlarm) in
        return (alarm.structuredLocation != nil) && ((alarm.proximity == .enter) || (alarm.proximity == .leave))
    }).isEmpty
}
```

### Sort Reminders

Retrieving reminders from the Calendar database returns reminders sorted by creation date. To sort an array of `EKReminder` objects by title, or any other property, the sample implements sorted(by:) on the array with a predicate that uses the property.

```
 /// - Returns: An array of reminders sorted by title in an ascending order.
func sortedByTitle() -> [EKReminder] {
    return self.sorted(by: { (first: EKReminder, second: EKReminder) in
        first.title.localizedCaseInsensitiveCompare(second.title) == .orderedAscending
    })
}
```

## See Also

### Events and reminders

Creating events and reminders

Create and modify events and reminders in a person’s database.

Retrieving events and reminders

Fetch events and reminders from the Calendar database.

Updating with notifications

Register for notifications about changes and keep your app up to date.

class EKEvent

A class that represents an event in a calendar.

class EKReminder

A class that represents a reminder in a calendar.

