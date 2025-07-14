

- SwiftUI
-  LabelStyleConfiguration 

Structure

# LabelStyleConfiguration

The properties of a label.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct LabelStyleConfiguration
```

## Topics

### Setting the icon

var icon: LabelStyleConfiguration.Icon

A symbolic representation of the labeled item.

struct Icon

A type-erased icon view of a label.

### Setting the title

var title: LabelStyleConfiguration.Title

A description of the labeled item.

struct Title

A type-erased title view of a label.

## See Also

### Styling views that display text

func labelStyle&lt;S>(S) -> some View

Sets the style for labels within this view.

protocol LabelStyle

A type that applies a custom appearance to all labels within a view.

func textFieldStyle&lt;S>(S) -> some View

Sets the style for text fields within this view.

protocol TextFieldStyle

A specification for the appearance and interaction of a text field.

func textEditorStyle(some TextEditorStyle) -> some View

Sets the style for text editors within this view.

protocol TextEditorStyle

A specification for the appearance and interaction of a text editor.

struct TextEditorStyleConfiguration

The properties of a text editor.

