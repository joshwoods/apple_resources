

- SwiftUI
- DatePickerStyle
-  DatePickerStyle.Configuration 

Type Alias

# DatePickerStyle.Configuration

A type alias for the properties of a `DatePicker`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 10.0+

``` source
typealias Configuration = DatePickerStyleConfiguration
```

## See Also

### Creating custom date picker styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Returns the appearance and interaction content for a `DatePicker`.

**Required**

struct DatePickerStyleConfiguration

The properties of a `DatePicker`.

associatedtype Body : View

A view representing the appearance and interaction of a `DatePicker`.

**Required**

