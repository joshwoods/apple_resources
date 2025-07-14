

- SwiftUI
- Text
-  foregroundColor(\_:) Deprecated

Instance Method

# foregroundColor(\_:)

Sets the color of the text displayed by this view.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
func foregroundColor(_ color: Color?) -> Text
```

Deprecated

Use foregroundStyle(_:) instead.

## Parameters 

`color`  

The color to use when displaying this text.

## Return Value

A text view that uses the color value you supply.

## Discussion

Use this method to change the color of the text rendered by a text view.

For example, you can display the names of the colors red, green, and blue in their respective colors:

```
HStack {
    Text("Red").foregroundColor(.red)
    Text("Green").foregroundColor(.green)
    Text("Blue").foregroundColor(.blue)
}
```

