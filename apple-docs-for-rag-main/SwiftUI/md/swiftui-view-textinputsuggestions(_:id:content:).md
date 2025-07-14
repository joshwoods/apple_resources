

- SwiftUI
- View
-  textInputSuggestions(\_:id:content:) 

Instance Method

# textInputSuggestions(\_:id:content:)

Configures the text input suggestions for this view.

macOS 15.0+

``` source
nonisolated
func textInputSuggestions(
    _ data: Data,
    id: KeyPath,
    @ViewBuilder content: @escaping (Data.Element) -> Content
) -> some View where Data : RandomAccessCollection, ID : Hashable, Content : View
```

## Parameters 

`data`  

The data that is used to create views dynamically.

`id`  

The key path to the provided data’s identifier.

`content`  

The view builder that creates views dynamically.

## Discussion

You can suggest text completions during a text input operation by providing data to this modifier. The interface presents the suggestion views as a list of choices when someone activates the text editing interface.

Associate a string with each suggestion view by adding the textInputCompletion(_:) modifier to the view.

Use `Label` to get platform-standard visual representations of suggestion text accompanied with images, and `Section` for labelled sections of results.

## See Also

### Managing text entry

func autocorrectionDisabled(Bool) -> some View

Sets whether to disable autocorrection for this view.

var autocorrectionDisabled: Bool

A Boolean value that determines whether the view hierarchy has auto-correction enabled.

func keyboardType(UIKeyboardType) -> some View

Sets the keyboard type for this view.

func scrollDismissesKeyboard(ScrollDismissesKeyboardMode) -> some View

Configures the behavior in which scrollable content interacts with the software keyboard.

func textContentType(_:)

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on macOS.

func textInputAutocapitalization(TextInputAutocapitalization?) -> some View

Sets how often the shift key in the keyboard is automatically enabled.

struct TextInputAutocapitalization

The kind of autocapitalization behavior applied during text input.

func textInputCompletion(String) -> some View

Associates a fully formed string with the value of this view when used as a text input suggestion

func textInputSuggestions&lt;S>(() -> S) -> some View

Configures the text input suggestions for this view.

func textInputSuggestions&lt;Data, Content>(Data, content: (Data.Element) -> Content) -> some View

Configures the text input suggestions for this view.

func textContentType(WKTextContentType?) -> some View

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on a watchOS device.

func textContentType(NSTextContentType?) -> some View

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on macOS.

func textContentType(UITextContentType?) -> some View

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on an iOS or tvOS device.

