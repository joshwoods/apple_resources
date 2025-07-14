

- FinanceKitUI
- AddOrderToWalletButton
-  presentationDragIndicator(\_:) 

Instance Method

# presentationDragIndicator(\_:)

Sets the visibility of the drag indicator on top of a sheet.

FinanceKitUISwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
nonisolated
func presentationDragIndicator(_ visibility: Visibility) -> some View
```

## Parameters 

`visibility`  

The preferred visibility of the drag indicator.

## Discussion

You can show a drag indicator when it isn’t apparent that a sheet can resize or when the sheet can’t dismiss interactively.

```
struct ContentView: View {
    @State private var showSettings = false

    var body: some View {
        Button("View Settings") {
            showSettings = true
        }
        .sheet(isPresented: $showSettings) {
            SettingsView()
                .presentationDetents([.medium, .large])
                .presentationDragIndicator(.visible)
        }
    }
}
```

