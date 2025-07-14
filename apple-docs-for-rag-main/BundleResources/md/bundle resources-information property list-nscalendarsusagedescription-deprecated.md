

- Bundle Resources
- Information Property List
-  NSCalendarsUsageDescription Deprecated

Property List Key

# NSCalendarsUsageDescription

A message that tells people why the app is requesting access to their calendar data.

iOS 6.0–17.0DeprecatediPadOS 6.0–17.0DeprecatedMac Catalyst 13.0–17.0DeprecatedmacOS 10.14–14.0DeprecatedwatchOS 6.0–10.0Deprecated

Deprecated

`NSCalendarsUsageDescription` has been deprecated. If your app needs read and write access to a person’s calendar data, use NSCalendarsFullAccessUsageDescription instead. If your app needs to create events in a person’s default calendar, use NSCalendarsWriteOnlyAccessUsageDescription instead.

## Details 

Name  
Privacy - Calendars Usage Description

Type  

string

## Discussion

Important

This key is required if your app uses APIs that access the person’s calendar data.

## See Also

### Deprecated keys

NSRemindersUsageDescription

A message that tells people why the app is requesting access to their reminders.

**Name:** Privacy - Reminders Usage Description

Deprecated

