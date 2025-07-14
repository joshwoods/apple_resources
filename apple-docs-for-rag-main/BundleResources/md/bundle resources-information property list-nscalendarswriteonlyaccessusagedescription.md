

- Bundle Resources
- Information Property List
-  NSCalendarsWriteOnlyAccessUsageDescription 

Property List Key

# NSCalendarsWriteOnlyAccessUsageDescription

A message that tells people why the app is requesting access to create calendar events.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+watchOS 10.0+

## Details 

Name  
Privacy - Calendars Write Only Usage Description

Type  

string

## Discussion

If your app needs to read calendar events in addition to creating them, use NSCalendarsFullAccessUsageDescription. If your app runs on iOS 17 or later and presents an EKEventEditViewController to allow people to create calendar events, you don’t need to request calendar access.

Important

This key is required if your app uses APIs that write to the person’s calendar data.

## See Also

### Calendar and reminders

NSCalendarsFullAccessUsageDescription

A message that tells people why the app is requesting access to read and write their calendar data.

**Name:** Privacy - Calendars Full Access Usage Description

NSRemindersFullAccessUsageDescription

A message that tells people why the app is requesting access to read and write their reminders data.

**Name:** Privacy - Reminders Full Access Usage Description

Accessing the event store

Request access to a person’s calendar data through the event store.

