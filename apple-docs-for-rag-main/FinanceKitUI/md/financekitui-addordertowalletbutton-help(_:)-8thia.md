

- FinanceKitUI
- AddOrderToWalletButton
-  help(\_:) 

Instance Method

# help(\_:)

Adds help text to a view using a text view that you provide.

FinanceKitUISwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func help(_ text: Text) -> some View
```

## Parameters 

`text`  

The `Text` view to use as help.

## Discussion

Adding help to a view configures the view’s accessibility hint and its help tag (also called a *tooltip*) in macOS or visionOS. For more information on using help tags, see Offering help in the Human Interface Guidelines.

```
Slider("Opacity", value: $selectedShape.opacity)
    .help(Text("Adjust the opacity of the selected \(selectedShape.name)"))
```

