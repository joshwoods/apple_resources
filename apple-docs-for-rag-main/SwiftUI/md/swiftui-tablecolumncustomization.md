

- SwiftUI
-  TableColumnCustomization 

Structure

# TableColumnCustomization

A representation of the state of the columns in a table.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
struct TableColumnCustomization where RowValue : Identifiable
```

## Overview

`TableColumnCustomization` can be created and provided to a table to enable column reordering and column visibility. The state can be queried and updated programmatically, as well as bound to persistent app or scene storage.

```
struct BugReportTable: View {
    @ObservedObject var dataModel: DataModel
    @Binding var selectedBugReports: Set

    @SceneStorage("BugReportTableConfig")
    private var columnCustomization: TableColumnCustomization

    var body: some View {
        Table(dataModel.bugReports, selection: $selectedBugReports,
            sortOrder: $dataModel.sortOrder,
            columnCustomization: $columnCustomization
        ) {
            TableColumn("Title", value: \.title)
                .customizationID("title")
            TableColumn("ID", value: \.id) {
                Link("\($0.id)", destination: $0.url)
            }
            .customizationID("id")
            TableColumn("Number of Reports", value: \.duplicateCount) {
                Text($0.duplicateCount, format: .number)
            }
            .customizationID("duplicates")
        }
    }
}
```

The above example creates a table with three columns. On macOS, these columns can be reordered or hidden and shown by the user of the app. Their configuration will be saved and restored with the window on relaunches of the app, using the “BugReportTableConfig” scene storage identifier.

The state of a specific column is stored relative to its customization identifier, using using the value from the customizationID(_:) modifier. When column customization is encoded and decoded, it relies on stable identifiers to restore the associate the saved state with a specific column. If a table column does not have a customization identifier, it will not be customizable.

These identifiers can also be used to programmatically change column customizations, such as programmatically hiding a column:

```
columnCustomization[visibility: "duplicates"] = .hidden
```

With a binding to the overall customization, a binding to the visibility of a column can be accessed using the same subscript syntax:

```
struct BugReportTable: View {
    @SceneStorage("BugReportTableConfig")
    private var columnCustomization: TableColumnCustomization

    var body: some View {
        ...
        MyVisibilityView($columnCustomization[visibility: "duplicates"])
    }
}

struct MyVisibilityView: View {
    @Binding var visibility: Visibility
    ...
}
```

## Topics

### Creating a table column customization

init()

Creates an empty table column customization.

### Managing the customization

func resetOrder()

Resets the column order back to the default, preserving the customized visibility and size.

subscript(visibility _: String) -> Visibility

The visibility of the column identified by its identifier.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Sendable

## See Also

### Customizing columns

func tableColumnHeaders(Visibility) -> some View

Controls the visibility of a `Table`’s column header views.

struct TableColumnCustomizationBehavior

A set of customization behaviors of a column that a table can offer to a user.

