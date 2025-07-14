

- SwiftUI
- View
-  textContentType(\_:) 

Instance Method

# textContentType(\_:)

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on an iOS or tvOS device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
nonisolated
func textContentType(_ textContentType: UITextContentType?) -> some View
```

Show all declarations

## Parameters 

`textContentType`  

One of the content types available in the UITextContentType structure that identify the semantic meaning expected for a text-entry area. These include support for email addresses, location names, URLs, and telephone numbers, to name just a few.

## Discussion

Use this method to set the content type for input text. For example, you can configure a TextField for the entry of email addresses:

```
TextField("Enter your email", text: $emailAddress)
    .textContentType(.emailAddress)
```

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

func textInputSuggestions&lt;Data, ID, Content>(Data, id: KeyPath&lt;Data.Element, ID>, content: (Data.Element) -> Content) -> some View

Configures the text input suggestions for this view.

func textContentType(WKTextContentType?) -> some View

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on a watchOS device.

func textContentType(NSTextContentType?) -> some View

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on macOS.

