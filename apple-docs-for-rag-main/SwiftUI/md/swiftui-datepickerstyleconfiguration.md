

- SwiftUI
-  DatePickerStyleConfiguration 

Structure

# DatePickerStyleConfiguration

The properties of a `DatePicker`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 10.0+

``` source
struct DatePickerStyleConfiguration
```

## Topics

### Establishing the date range

var minimumDate: Date?

The oldest selectable date.

var maximumDate: Date?

The most recent selectable date.

### Labeling the date picker

let label: DatePickerStyleConfiguration.Label

A description of the `DatePicker`.

struct Label

A type-erased label of a `DatePicker`.

var displayedComponents: DatePickerComponents

The date components that the user is able to view and edit.

### Selecting the date

var selection: Date

The date value being displayed and selected.

var $selection: Binding&lt;Date>

## See Also

### Creating custom date picker styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Returns the appearance and interaction content for a `DatePicker`.

**Required**

typealias Configuration

A type alias for the properties of a `DatePicker`.

associatedtype Body : View

A view representing the appearance and interaction of a `DatePicker`.

**Required**

