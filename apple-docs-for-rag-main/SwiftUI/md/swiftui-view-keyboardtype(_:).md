

- SwiftUI
- View
-  keyboardType(\_:) 

Instance Method

# keyboardType(\_:)

Sets the keyboard type for this view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
nonisolated
func keyboardType(_ type: UIKeyboardType) -> some View
```

## Parameters 

`type`  

One of the keyboard types defined in the UIKeyboardType enumeration.

## Discussion

Use `keyboardType(_:)` to specify the keyboard type to use for text entry. A number of different keyboard types are available to meet specialized input needs, such as entering email addresses or phone numbers.

The example below presents a TextField to input an email address. Setting the text field’s keyboard type to `.emailAddress` ensures the user can only enter correctly formatted email addresses.

```
TextField("someone@example.com", text: $emailAddress)
    .keyboardType(.emailAddress)
```

There are several different kinds of specialized keyboard types available though the UIKeyboardType enumeration. To specify the default system keyboard type, use `.default`.

## See Also

### Managing text entry

func autocorrectionDisabled(Bool) -> some View

Sets whether to disable autocorrection for this view.

var autocorrectionDisabled: Bool

A Boolean value that determines whether the view hierarchy has auto-correction enabled.

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

func textContentType(UITextContentType?) -> some View

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on an iOS or tvOS device.

