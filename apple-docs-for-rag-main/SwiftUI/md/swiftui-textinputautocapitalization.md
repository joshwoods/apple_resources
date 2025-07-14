

- SwiftUI
-  TextInputAutocapitalization 

Structure

# TextInputAutocapitalization

The kind of autocapitalization behavior applied during text input.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct TextInputAutocapitalization
```

## Overview

Pass an instance of `TextInputAutocapitalization` to the textInputAutocapitalization(_:) view modifier.

## Topics

### Getting autocapitalization options

static var characters: TextInputAutocapitalization

Defines an autocapitalizing behavior that will capitalize every letter.

static var sentences: TextInputAutocapitalization

Defines an autocapitalizing behavior that will capitalize the first letter in every sentence.

static var words: TextInputAutocapitalization

Defines an autocapitalizing behavior that will capitalize the first letter of every word.

static var never: TextInputAutocapitalization

Defines an autocapitalizing behavior that will not capitalize anything.

### Creating an autocapitalization type

init?(UITextAutocapitalizationType)

Creates a new TextInputAutocapitalization struct from a `UITextAutocapitalizationType` enum.

## Relationships

### Conforms To

- Sendable

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

