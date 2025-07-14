

- EventKit UI
- EKCalendarChooser
-  init(selectionStyle:displayStyle:eventStore:) 

Initializer

# init(selectionStyle:displayStyle:eventStore:)

Initializes a newly created calendar chooser.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
@MainActor
init(
    selectionStyle: EKCalendarChooserSelectionStyle,
    displayStyle: EKCalendarChooserDisplayStyle,
    eventStore: EKEventStore
)
```

## Parameters 

`selectionStyle`  

Determines whether to allow selection of multiple calendars. Possible values are described in EKCalendarChooserSelectionStyle.

`displayStyle`  

Determines which calendars to display. Possible values are described in EKCalendarChooserDisplayStyle.

`eventStore`  

The event store to which the calendars belong.

## Return Value

The initialized calendar chooser.

## See Also

### Initializing Calendar Choosers

init(selectionStyle: EKCalendarChooserSelectionStyle, displayStyle: EKCalendarChooserDisplayStyle, entityType: EKEntityType, eventStore: EKEventStore)

Initializes a newly created calendar chooser for a specific entity type.

