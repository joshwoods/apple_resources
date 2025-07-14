

- MusicKit
- ArtworkImage
-  toolbarRole(\_:) 

Instance Method

# toolbarRole(\_:)

Configures the semantic role for the content populating the toolbar.

MusicKitSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func toolbarRole(_ role: ToolbarRole) -> some View
```

## Parameters 

`role`  

The role of the toolbar.

## Discussion

Use this modifier to configure the semantic role for content populating your app’s toolbar. SwiftUI uses this role when rendering the content of your app’s toolbar.

```
ContentView()
    .navigationTitle("Browser")
    .toolbarRole(.browser)
    .toolbar {
        ToolbarItem(placement: .primaryAction) {
            AddButton()
        }
     }
```

