

- SwiftUI
- ToolbarContent
-  hidden(\_:) 

Instance Method

# hidden(\_:)

Hides a toolbar item within its toolbar.

macOS 15.0+

``` source
nonisolated
func hidden(_ hidden: Bool = true) -> some ToolbarContent
```

## Parameters 

`hidden`  

Whether the toolbar item is hidden.

## Discussion

Use this modifier to conditionally display a toolbar item in its toolbar.

```
struct ContentView {
    @State private var showDownloads = false

    var body: some View {
        BrowserView()
            .toolbar {
                ToolbarItem {
                    DownloadsButton()
                }
                .hidden(!showDownloads)
            }
    }
}
```

