

- UIKit
- UICalendarViewDelegate
-  calendarView(\_:decorationFor:) 

Instance Method

# calendarView(\_:decorationFor:)

Creates a calendar view decoration for the date represented by the date components you provide.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
optional func calendarView(
    _ calendarView: UICalendarView,
    decorationFor dateComponents: DateComponents
) -> UICalendarView.Decoration?
```

## Parameters 

`calendarView`  

The calendar view object requesting the decoration.

`dateComponents`  

Date components that represent the date for the calendar view to display a decoration.

## Return Value

A calendar view decoration.

