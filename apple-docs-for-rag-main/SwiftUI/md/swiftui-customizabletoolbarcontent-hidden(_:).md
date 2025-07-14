

- SwiftUI
- CustomizableToolbarContent
-  hidden(\_:) 

Instance Method

# hidden(\_:)

Hides a toolbar item within its toolbar.

macOS 15.0+

``` source
nonisolated
func hidden(_ hidden: Bool = true) -> some CustomizableToolbarContent
```

## Parameters 

`hidden`  

Whether the toolbar item is hidden.

## Discussion

Use this modifier to conditionally display a toolbar item in its toolbar. On macOS and iOS, hidden items will be displayed during user customization.

The following example hides a downloads button when there are no downloads, but it is displayed during customization.

```
struct ContentView {
    @State private var showDownloads = false

    var body: some View {
        BrowserView()
            .toolbar(id: "browserToolbar") {
                ToolbarItem(id: "downloads") {
                    DownloadsButton()
                }
                .hidden(!showDownloads)
            }
    }
}
```

