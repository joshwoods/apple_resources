

- SwiftUI
- DatePickerStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Returns the appearance and interaction content for a `DatePicker`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 10.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## Discussion

The system calls this method for each DatePicker instance in a view hierarchy where this style is the current date picker style.

## See Also

### Creating custom date picker styles

struct DatePickerStyleConfiguration

The properties of a `DatePicker`.

typealias Configuration

A type alias for the properties of a `DatePicker`.

associatedtype Body : View

A view representing the appearance and interaction of a `DatePicker`.

**Required**

