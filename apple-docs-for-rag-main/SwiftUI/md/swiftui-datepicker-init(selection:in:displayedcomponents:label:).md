

- SwiftUI
- DatePicker
-  init(selection:in:displayedComponents:label:) 

Initializer

# init(selection:in:displayedComponents:label:)

Creates an instance that selects a `Date` in a closed range.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    selection: Binding,
    in range: ClosedRange,
    displayedComponents: DatePicker.Components = [.hourAndMinute, .date],
    @ViewBuilder label: () -> Label
)
```

Available when `Label` conforms to `View`.

Show all declarations

## Parameters 

`selection`  

The date value being displayed and selected.

`range`  

The inclusive range of selectable dates.

`displayedComponents`  

The date components that user is able to view and edit. Defaults to `[.hourAndMinute, .date]`. On watchOS, if `.hourAndMinute` or `.hourMinuteAndSecond` are included with `.date`, only `.date` is displayed.

`label`  

A view that describes the use of the date.

## See Also

### Creating a date picker for specific dates

init(_:selection:in:displayedComponents:)

Creates an instance that selects a `Date` in a closed range.

