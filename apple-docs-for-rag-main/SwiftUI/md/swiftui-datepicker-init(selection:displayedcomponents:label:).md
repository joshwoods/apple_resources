

- SwiftUI
- DatePicker
-  init(selection:displayedComponents:label:) 

Initializer

# init(selection:displayedComponents:label:)

Creates an instance that selects a `Date` with an unbounded range.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    selection: Binding,
    displayedComponents: DatePicker.Components = [.hourAndMinute, .date],
    @ViewBuilder label: () -> Label
)
```

Available when `Label` conforms to `View`.

## Parameters 

`selection`  

The date value being displayed and selected.

`displayedComponents`  

The date components that user is able to view and edit. Defaults to `[.hourAndMinute, .date]`. On watchOS, if `.hourAndMinute` or `.hourMinuteAndSecond` are included with `.date`, only `.date` is displayed.

`label`  

A view that describes the use of the date.

## See Also

### Creating a date picker for any date

init(_:selection:displayedComponents:)

Creates an instance that selects a `Date` with an unbounded range.

