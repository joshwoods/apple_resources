

- EventKit
- EKError
-  calendarDoesNotAllowReminders 

Type Property

# calendarDoesNotAllowReminders

The calendar doesn’t allow you to add reminders.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
static var calendarDoesNotAllowReminders: EKError.Code { get }
```

## See Also

### Error Codes

static var eventNotMutable: EKError.Code

The event isn’t mutable and you can’t save or delete it.

static var noCalendar: EKError.Code

The event isn’t associated with a calendar.

static var noEndDate: EKError.Code

The event has no start date set.

static var noStartDate: EKError.Code

The event has no end date set.

static var datesInverted: EKError.Code

The event’s end date occurs before its start date.

static var internalFailure: EKError.Code

An internal error occurred.

static var calendarReadOnly: EKError.Code

The calendar is read-only and you can’t add events to it.

static var durationGreaterThanRecurrence: EKError.Code

The duration of an event is greater than its recurrence interval.

static var alarmGreaterThanRecurrence: EKError.Code

The alarm interval is greater than the recurrence interval.

static var startDateTooFarInFuture: EKError.Code

The start date is further into the future than the calendar can display.

static var startDateCollidesWithOtherOccurrence: EKError.Code

The event’s start date collides with another occurrence of the event.

static var objectBelongsToDifferentStore: EKError.Code

The object belongs to a different calendar store.

static var invitesCannotBeMoved: EKError.Code

You can’t move the event because it’s an invitation.

static var invalidSpan: EKError.Code

The system encountered an invalid span during a save or deletion.

static var calendarHasNoSource: EKError.Code

You can’t save the calendar without setting a source first.

