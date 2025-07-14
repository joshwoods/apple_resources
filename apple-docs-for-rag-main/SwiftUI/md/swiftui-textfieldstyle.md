

- SwiftUI
-  TextFieldStyle 

Protocol

# TextFieldStyle

A specification for the appearance and interaction of a text field.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol TextFieldStyle
```

## Topics

### Getting built-in text field styles

static var automatic: DefaultTextFieldStyle

The default text field style, based on the text field’s context.

static var plain: PlainTextFieldStyle

A text field style with no decoration.

static var roundedBorder: RoundedBorderTextFieldStyle

A text field style with a system-defined rounded border.

static var squareBorder: SquareBorderTextFieldStyle

A text field style with a system-defined square border.

### Supporting types

struct DefaultTextFieldStyle

The default text field style, based on the text field’s context.

struct PlainTextFieldStyle

A text field style with no decoration.

struct RoundedBorderTextFieldStyle

A text field style with a system-defined rounded border.

struct SquareBorderTextFieldStyle

A text field style with a system-defined square border.

## Relationships

### Conforming Types

- DefaultTextFieldStyle
- PlainTextFieldStyle
- RoundedBorderTextFieldStyle
- SquareBorderTextFieldStyle

## See Also

### Styling views that display text

func labelStyle&lt;S>(S) -> some View

Sets the style for labels within this view.

protocol LabelStyle

A type that applies a custom appearance to all labels within a view.

struct LabelStyleConfiguration

The properties of a label.

func textFieldStyle&lt;S>(S) -> some View

Sets the style for text fields within this view.

func textEditorStyle(some TextEditorStyle) -> some View

Sets the style for text editors within this view.

protocol TextEditorStyle

A specification for the appearance and interaction of a text editor.

struct TextEditorStyleConfiguration

The properties of a text editor.

