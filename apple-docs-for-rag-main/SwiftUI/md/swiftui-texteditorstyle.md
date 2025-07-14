

- SwiftUI
-  TextEditorStyle 

Protocol

# TextEditorStyle

A specification for the appearance and interaction of a text editor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
protocol TextEditorStyle
```

## Overview

A type conforming to this protocol inherits `@preconcurrency @MainActor` isolation from the protocol if the conformance is included in the type’s base declaration:

```
struct MyCustomType: Transition {
    // `@preconcurrency @MainActor` isolation by default
}
```

Isolation to the main actor is the default, but it’s not required. Declare the conformance in an extension to opt out of main actor isolation:

```
extension MyCustomType: Transition {
    // `nonisolated` by default
}
```

## Topics

### Getting built-in styles

static var automatic: AutomaticTextEditorStyle

The default text editor style, based on the text editor’s context.

static var plain: PlainTextEditorStyle

A text editor style with no decoration.

static var roundedBorder: RoundedBorderTextEditorStyle

A text editor style with a system-defined rounded border.

### Creating custom styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a text editor.

**Required**

typealias Configuration

The properties of a text editor.

associatedtype Body : View

A view that represents the body of a text editor.

**Required**

### Supporting types

struct AutomaticTextEditorStyle

The default text editor style, based on the text editor’s context.

struct PlainTextEditorStyle

A text editor style with no decoration.

struct RoundedBorderTextEditorStyle

A text editor style with a system-defined rounded border.

## Relationships

### Conforming Types

- AutomaticTextEditorStyle
- PlainTextEditorStyle
- RoundedBorderTextEditorStyle

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

protocol TextFieldStyle

A specification for the appearance and interaction of a text field.

func textEditorStyle(some TextEditorStyle) -> some View

Sets the style for text editors within this view.

struct TextEditorStyleConfiguration

The properties of a text editor.

