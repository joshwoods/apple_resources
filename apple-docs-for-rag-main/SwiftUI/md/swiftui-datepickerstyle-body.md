

- SwiftUI
- DatePickerStyle
-  Body 

Associated Type

# Body

A view representing the appearance and interaction of a `DatePicker`.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 10.0+

``` source
associatedtype Body : View
```

**Required**

## See Also

### Creating custom date picker styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Returns the appearance and interaction content for a `DatePicker`.

**Required**

struct DatePickerStyleConfiguration

The properties of a `DatePicker`.

typealias Configuration

A type alias for the properties of a `DatePicker`.

