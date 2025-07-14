

- SwiftUI
- View
-  alert(item:content:) Deprecated

Instance Method

# alert(item:content:)

Presents an alert to the user.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
func alert(
    item: Binding,
    content: (Item) -> Alert
) -> some View where Item : Identifiable
```

Deprecated

Use alert(_:isPresented:presenting:actions:message:) instead.

## Parameters 

`item`  

A binding to an optional source of truth for the alert. if `item` is non-`nil`, the system passes the contents to the modifier’s closure. You use this content to populate the fields of an alert that you create that the system displays to the user. If `item` changes, the system dismisses the currently displayed alert and replaces it with a new one using the same process.

`content`  

A closure returning the alert to present.

## Discussion

Use this method when you need to show an alert that contains information from a binding to an optional data source that you provide. The example below shows a custom data source `FileInfo` whose properties configure the alert’s `message` field:

```
struct FileInfo: Identifiable {
    var id: String { name }
    let name: String
    let fileType: UTType
}

struct ConfirmImportAlert: View {
    @State private var alertDetails: FileInfo?
    var body: some View {
        Button("Show Alert") {
            alertDetails = FileInfo(name: "MyImageFile.png",
                                    fileType: .png)
        }
        .alert(item: $alertDetails) { details in
            Alert(title: Text("Import Complete"),
                  message: Text("""
                    Imported \(details.name) \n File
                    type: \(details.fileType.description).
                    """),
                  dismissButton: .default(Text("Dismiss")))
        }
    }
}
```

## See Also

### View presentation modifiers

func actionSheet(isPresented: Binding&lt;Bool>, content: () -> ActionSheet) -> some View

Presents an action sheet when a given condition is true.

Deprecated

func actionSheet&lt;T>(item: Binding&lt;T?>, content: (T) -> ActionSheet) -> some View

Presents an action sheet using the given item as a data source for the sheet’s content.

Deprecated

func alert(isPresented: Binding&lt;Bool>, content: () -> Alert) -> some View

Presents an alert to the user.

Deprecated

