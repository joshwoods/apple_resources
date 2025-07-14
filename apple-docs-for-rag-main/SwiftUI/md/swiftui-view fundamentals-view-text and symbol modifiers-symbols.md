

- SwiftUI
- View fundamentals
- View
-  Text and symbol modifiers 

API Collection

# Text and symbol modifiers

Manage the rendering, selection, and entry of text in your view.

## Overview

SwiftUI provides built-in views that display text to the user, like Text and Label, or that collect text from the user, like TextField and TextEditor. Use text and symbol modifiers to control how SwiftUI displays and manages that text. For example, you can set a font, specify text layout parameters, and indicate what kind of input to expect.

To learn more about the kinds of views that you use to display text and the ways in which you can configure those views, see Text input and output.

## Topics

### Fonts

func font(Font?) -> some View

Sets the default font for text in this view.

### Dynamic type

func dynamicTypeSize(_:)

Sets the Dynamic Type size within the view to the given value.

### Text style

func bold(Bool) -> some View

Applies a bold font weight to the text in this view.

func fontDesign(Font.Design?) -> some View

Sets the font design of the text in this view.

func fontWeight(Font.Weight?) -> some View

Sets the font weight of the text in this view.

func fontWidth(Font.Width?) -> some View

Sets the font width of the text in this view.

func italic(Bool) -> some View

Applies italics to the text in this view.

func monospaced(Bool) -> some View

Modifies the fonts of all child views to use the fixed-width variant of the current font, if possible.

func monospacedDigit() -> some View

Modifies the fonts of all child views to use fixed-width digits, if possible, while leaving other characters proportionally spaced.

func strikethrough(Bool, pattern: Text.LineStyle.Pattern, color: Color?) -> some View

Applies a strikethrough to the text in this view.

func textCase(Text.Case?) -> some View

Sets a transform for the case of the text contained in this view when displayed.

func textScale(Text.Scale, isEnabled: Bool) -> some View

Applies a text scale to text in the view.

func underline(Bool, pattern: Text.LineStyle.Pattern, color: Color?) -> some View

Applies an underline to the text in this view.

### Text layout

func allowsTightening(Bool) -> some View

Sets whether text in this view can compress the space between characters when necessary to fit text in a line.

func baselineOffset(CGFloat) -> some View

Sets the vertical offset for the text relative to its baseline in this view.

func flipsForRightToLeftLayoutDirection(Bool) -> some View

Sets whether this view mirrors its contents horizontally when the layout direction is right-to-left.

func kerning(CGFloat) -> some View

Sets the spacing, or kerning, between characters for the text in this view.

func minimumScaleFactor(CGFloat) -> some View

Sets the minimum amount that text in this view scales down to fit in the available space.

func tracking(CGFloat) -> some View

Sets the tracking for the text in this view.

func truncationMode(Text.TruncationMode) -> some View

Sets the truncation mode for lines of text that are too long to fit in the available space.

func typesettingLanguage(_:isEnabled:)

Specifies the language for typesetting.

### Multiline text

func lineLimit(_:)

Sets to a closed range the number of lines that text can occupy in this view.

func lineLimit(Int, reservesSpace: Bool) -> some View

Sets a limit for the number of lines text can occupy in this view.

func lineSpacing(CGFloat) -> some View

Sets the amount of space between lines of text in this view.

func multilineTextAlignment(TextAlignment) -> some View

Sets the alignment of a text view that contains multiple lines of text.

### Text selection

func textSelection&lt;S>(S) -> some View

Controls whether people can select text within this view.

### Text entry

func autocorrectionDisabled(Bool) -> some View

Sets whether to disable autocorrection for this view.

func keyboardType(UIKeyboardType) -> some View

Sets the keyboard type for this view.

func scrollDismissesKeyboard(ScrollDismissesKeyboardMode) -> some View

Configures the behavior in which scrollable content interacts with the software keyboard.

func textInputAutocapitalization(TextInputAutocapitalization?) -> some View

Sets how often the shift key in the keyboard is automatically enabled.

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

### Find and replace

func findNavigator(isPresented: Binding&lt;Bool>) -> some View

Programmatically presents the find and replace interface for text editor views.

func findDisabled(Bool) -> some View

Prevents find and replace operations in a text editor.

func replaceDisabled(Bool) -> some View

Prevents replace operations in a text editor.

### Symbol appearance

func symbolRenderingMode(SymbolRenderingMode?) -> some View

Sets the rendering mode for symbol images within this view.

func symbolVariant(SymbolVariants) -> some View

Makes symbols within the view show a particular variant.

## See Also

### Configuring view elements

Accessibility modifiers

Make your SwiftUI apps accessible to everyone, including people with disabilities.

Appearance modifiers

Configure a view’s foreground and background styles, controls, and visibility.

Auxiliary view modifiers

Add and configure supporting views, like toolbars and context menus.

Chart view modifiers

Configure charts that you declare with Swift Charts.

