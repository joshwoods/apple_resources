

- SwiftUI
- DatePicker
-  init(\_:selection:displayedComponents:) 

Initializer

# init(\_:selection:displayedComponents:)

Creates an instance that selects a `Date` with an unbounded range.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    selection: Binding,
    displayedComponents: DatePicker.Components = [.hourAndMinute, .date]
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the localized title of `self`, describing its purpose.

`selection`  

The date value being displayed and selected.

`displayedComponents`  

The date components that user is able to view and edit. Defaults to `[.hourAndMinute, .date]`. On watchOS, if `.hourAndMinute` or `.hourMinuteAndSecond` are included with `.date`, only `.date` is displayed.

## See Also

### Creating a date picker for any date

init(selection: Binding&lt;Date>, displayedComponents: DatePicker&lt;Label>.Components, label: () -> Label)

Creates an instance that selects a `Date` with an unbounded range.

