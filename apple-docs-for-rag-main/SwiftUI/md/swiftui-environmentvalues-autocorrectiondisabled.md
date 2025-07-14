

- SwiftUI
- EnvironmentValues
-  autocorrectionDisabled 

Instance Property

# autocorrectionDisabled

A Boolean value that determines whether the view hierarchy has auto-correction enabled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 8.0+

``` source
var autocorrectionDisabled: Bool { get set }
```

## Discussion

The default value is `false`.

## See Also

### Managing text entry

func autocorrectionDisabled(Bool) -> some View

Sets whether to disable autocorrection for this view.

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

func textContentType(UITextContentType?) -> some View

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on an iOS or tvOS device.

