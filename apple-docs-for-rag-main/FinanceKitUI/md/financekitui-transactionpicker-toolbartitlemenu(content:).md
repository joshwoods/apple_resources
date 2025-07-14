

- FinanceKitUI
- TransactionPicker
-  toolbarTitleMenu(content:) 

Instance Method

# toolbarTitleMenu(content:)

Configure the title menu of a toolbar.

FinanceKitUISwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
nonisolated
func toolbarTitleMenu(@ViewBuilder content: () -> C) -> some View where C : View
```

## Parameters 

`content`  

The content associated to the toolbar title menu.

## Discussion

A title menu represent common functionality that can be done on the content represented by your app’s toolbar or navigation title. This menu may be populated from your app’s commands like `CommandGroupPlacement/saveItem` or `CommandGroupPlacement/printItem`.

```
ContentView()
    .toolbar {
        ToolbarTitleMenu()
    }
```

You can provide your own set of actions to override this behavior.

```
ContentView()
    .toolbarTitleMenu {
        DuplicateButton()
        PrintButton()
    }
```

In iOS and iPadOS, this will construct a menu that can be presented by tapping the navigation title in the app’s navigation bar.

