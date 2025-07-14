

- FinanceKitUI
- TransactionPicker
-  widgetURL(\_:) 

Instance Method

# widgetURL(\_:)

Sets the URL to open in the containing app when the user clicks the widget.

FinanceKitUISwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
func widgetURL(_ url: URL?) -> some View
```

## Parameters 

`url`  

The URL to open in the containing app.

## Return Value

A view that opens the specified URL when the user clicks the widget.

## Discussion

Widgets support one `widgetURL` modifier in their view hierarchy. If multiple views have `widgetURL` modifiers, the behavior is undefined.

