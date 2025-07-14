

- EventKit UI
- EKCalendarChooser
-  init(selectionStyle:displayStyle:entityType:eventStore:) 

Initializer

# init(selectionStyle:displayStyle:entityType:eventStore:)

Initializes a newly created calendar chooser for a specific entity type.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
@MainActor
init(
    selectionStyle style: EKCalendarChooserSelectionStyle,
    displayStyle: EKCalendarChooserDisplayStyle,
    entityType: EKEntityType,
    eventStore: EKEventStore
)
```

## Parameters 

`style`  

Determines whether to allow selection of multiple calendars. Possible values are described in EKCalendarChooserSelectionStyle.

`displayStyle`  

Determines which calendars to display. Possible values are described in EKCalendarChooserDisplayStyle.

`entityType`  

The entity type of the calendar. Possible values are EKEntityType.event and EKEntityType.reminder.

`eventStore`  

The event store to which the calendars belong.

## Return Value

The initialized calendar chooser.

## See Also

### Initializing Calendar Choosers

init(selectionStyle: EKCalendarChooserSelectionStyle, displayStyle: EKCalendarChooserDisplayStyle, eventStore: EKEventStore)

Initializes a newly created calendar chooser.

