

- SwiftUI
- TextEditorStyle
-  automatic 

Type Property

# automatic

The default text editor style, based on the text editor’s context.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
static var automatic: AutomaticTextEditorStyle { get }
```

Available when `Self` is `AutomaticTextEditorStyle`.

## Discussion

The default style represents the recommended style based on the current platform and the text editor’s context within the view hierarchy.

## See Also

### Getting built-in styles

static var plain: PlainTextEditorStyle

A text editor style with no decoration.

static var roundedBorder: RoundedBorderTextEditorStyle

A text editor style with a system-defined rounded border.

