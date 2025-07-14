

- SwiftUI
-  DatePicker 

Structure

# DatePicker

A control for selecting an absolute date.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 10.0+

``` source
struct DatePicker where Label : View
```

## Mentioned in 

Laying out a simple view

## Overview

Use a `DatePicker` when you want to provide a view that allows the user to select a calendar date, and optionally a time. The view binds to a Date instance.

The following example creates a basic `DatePicker`, which appears on iOS as text representing the date. This example limits the display to only the calendar date, not the time. When the user taps or clicks the text, a calendar view animates in, from which the user can select a date. When the user dismisses the calendar view, the view updates the bound Date.

```
@State private var date = Date()

var body: some View {
    DatePicker(
        "Start Date",
        selection: $date,
        displayedComponents: [.date]
    )
}
```

For cases where adding a subtitle to the label is desired, use a view builder that creates multiple `Text` views where the first text represents the title and the second text represents the subtitle:

```
@State private var date = Date()

var body: some View {
    DatePicker(selection: $date) {
        Text("Start Date")
        Text("Select the starting date for the event")
    }
}
```

You can limit the `DatePicker` to specific ranges of dates, allowing selections only before or after a certain date, or between two dates. The following example shows a date-and-time picker that only permits selections within the year 2021 (in the `UTC` time zone).

```
@State private var date = Date()
let dateRange: ClosedRange = {
    let calendar = Calendar.current
    let startComponents = DateComponents(year: 2021, month: 1, day: 1)
    let endComponents = DateComponents(year: 2021, month: 12, day: 31, hour: 23, minute: 59, second: 59)
    return calendar.date(from:startComponents)!
        ...
        calendar.date(from:endComponents)!
}()

var body: some View {
    DatePicker(
        "Start Date",
         selection: $date,
         in: dateRange,
         displayedComponents: [.date, .hourAndMinute]
    )
}
```

### Styling date pickers

To use a different style of date picker, use the datePickerStyle(_:) view modifier. The following example shows the graphical date picker style.

```
@State private var date = Date()

var body: some View {
    DatePicker(
        "Start Date",
        selection: $date,
        displayedComponents: [.date]
    )
    .datePickerStyle(.graphical)
}
```

## Topics

### Creating a date picker for any date

init(_:selection:displayedComponents:)

Creates an instance that selects a `Date` with an unbounded range.

init(selection: Binding&lt;Date>, displayedComponents: DatePicker&lt;Label>.Components, label: () -> Label)

Creates an instance that selects a `Date` with an unbounded range.

### Creating a date picker for specific dates

init(_:selection:in:displayedComponents:)

Creates an instance that selects a `Date` in a closed range.

init(selection:in:displayedComponents:label:)

Creates an instance that selects a `Date` in a closed range.

### Setting date picker components

typealias Components

struct DatePickerComponents

## Relationships

### Conforms To

- View

## See Also

### Choosing dates

func datePickerStyle&lt;S>(S) -> some View

Sets the style for date pickers within this view.

struct MultiDatePicker

A control for picking multiple dates.

var calendar: Calendar

The current calendar that views should use when handling dates.

var timeZone: TimeZone

The current time zone that views should use when handling dates.

