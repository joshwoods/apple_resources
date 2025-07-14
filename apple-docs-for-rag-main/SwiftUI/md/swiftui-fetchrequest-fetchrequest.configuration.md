

- SwiftUI
- FetchRequest
-  FetchRequest.Configuration 

Structure

# FetchRequest.Configuration

The request’s configurable properties.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
struct Configuration
```

## Overview

You initialize a FetchRequest with an optional predicate and sort descriptors, either explicitly or using a configured NSFetchRequest. Later, you can dynamically update the predicate and sort parameters using the request’s configuration structure.

You access or bind to a request’s configuration components through properties on the associated FetchedResults instance.

### Configure using a binding

Get a Binding to a fetch request’s configuration structure by accessing the request’s projectedValue, which you do by using the dollar sign (`$`) prefix on the associated results property. For example, you can create a request for `Quake` entities — a managed object type that the Loading and Displaying a Large Data Feed sample code project defines — that initially sorts the results by time:

```
@FetchRequest(sortDescriptors: [SortDescriptor(\.time, order: .reverse)])
private var quakes: FetchedResults
```

Then you can bind the request’s sort descriptors, which you access through the `quakes` result, to those of a Table instance:

```
Table(quakes, sortOrder: $quakes.sortDescriptors) {
    TableColumn("Place", value: \.place)
    TableColumn("Time", value: \.time) { quake in
        Text(quake.time, style: .time)
    }
}
```

A user who clicks on a table column header initiates the following sequence of events:

1.  The table updates the sort descriptors through the binding.

2.  The modified sort descriptors reconfigure the request.

3.  The reconfigured request fetches new results.

4.  SwiftUI redraws the table in response to new results.

### Set configuration directly

If you need to access the fetch request’s configuration elements directly, use the nsPredicate and sortDescriptors or nsSortDescriptors properties of the FetchedResults instance. Continuing the example above, to enable the user to dynamically update the predicate, declare a State property to hold a query string:

```
@State private var query = ""
```

Then add an onChange(of:initial:_:) modifier to the Table that sets a new predicate any time the query changes:

```
.onChange(of: query) { _, value in
    quakes.nsPredicate = query.isEmpty
        ? nil
        : NSPredicate(format: "place CONTAINS %@", value)
}
```

To give the user control over the string, add a TextField in your user interface that’s bound to the `query` state:

```
TextField("Filter", text: $query)
```

When the user types into the text field, the predicate updates, the request fetches new results, and SwiftUI redraws the table.

## Topics

### Setting a predicate

var nsPredicate: NSPredicate?

The request’s predicate.

### Setting sort descriptors

var sortDescriptors: [SortDescriptor&lt;Result>]

The request’s sort descriptors, accessed as value types.

var nsSortDescriptors: [NSSortDescriptor]

The request’s sort descriptors, accessed as reference types.

## Relationships

### Conforms To

- Sendable

## See Also

### Configuring a request dynamically

var projectedValue: Binding&lt;FetchRequest&lt;Result>.Configuration>

A binding to the request’s mutable configuration properties.

