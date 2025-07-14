

- FamilyControls
- FamilyActivityTitleView
-  scrollDismissesKeyboard(\_:) 

Instance Method

# scrollDismissesKeyboard(\_:)

Configures the behavior in which scrollable content interacts with the software keyboard.

FamilyControlsSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
nonisolated
func scrollDismissesKeyboard(_ mode: ScrollDismissesKeyboardMode) -> some View
```

## Parameters 

`mode`  

The keyboard dismissal mode that scrollable content uses.

## Return Value

A view that uses the specified keyboard dismissal mode.

## Discussion

You use this modifier to customize how scrollable content interacts with the software keyboard. For example, you can specify a value of `ScrollDismissesKeyboardMode/immediately` to indicate that you would like scrollable content to immediately dismiss the keyboard if present when a scroll drag gesture begins.

```
@State private var text = ""

ScrollView {
    TextField("Prompt", text: $text)
    ForEach(0 ..

You can also use this modifier to customize the keyboard dismissal behavior for other kinds of scrollable views, like a `List` or a `TextEditor`.

By default, a `TextEditor` is interactive while other kinds of scrollable content always dismiss the keyboard on a scroll when linked against iOS 16 or later. Pass a value of `ScrollDismissesKeyboardMode/never` to indicate that scrollable content should never automatically dismiss the keyboard.

