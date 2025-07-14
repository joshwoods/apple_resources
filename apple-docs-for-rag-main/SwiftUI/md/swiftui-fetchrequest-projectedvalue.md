

- SwiftUI
- FetchRequest
-  projectedValue 

Instance Property

# projectedValue

A binding to the request’s mutable configuration properties.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
var projectedValue: Binding.Configuration> { get }
```

## Discussion

SwiftUI returns the value associated with this property when you use FetchRequest as a property wrapper on a FetchedResults instance, and then access the results with a dollar sign (`$`) prefix. The value that SwiftUI returns is a Binding to the request’s FetchRequest.Configuration structure, which dynamically configures the request.

For example, consider the following fetch request for a type that the Loading and Displaying a Large Data Feed sample code project defines to store earthquake data, sorted based on the `time` property:

```
@FetchRequest(sortDescriptors: [SortDescriptor(\.time, order: .reverse)])
private var quakes: FetchedResults
```

You can use the projected value to enable a Table instance to make updates:

```
Table(quakes, sortOrder: $quakes.sortDescriptors) {
    TableColumn("Place", value: \.place)
    TableColumn("Time", value: \.time) { quake in
        Text(quake.time, style: .time)
    }
}
```

Because you initialize the table using a binding to the descriptors, the table can modify the sort in response to actions that the user takes, like clicking a column header.

## See Also

### Configuring a request dynamically

struct Configuration

The request’s configurable properties.

