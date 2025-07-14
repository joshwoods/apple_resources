

- SwiftUI
- TextFieldStyle
-  automatic 

Type Property

# automatic

The default text field style, based on the text field’s context.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var automatic: DefaultTextFieldStyle { get }
```

Available when `Self` is `DefaultTextFieldStyle`.

## Discussion

The default style represents the recommended style based on the current platform and the text field’s context within the view hierarchy.

## See Also

### Getting built-in text field styles

static var plain: PlainTextFieldStyle

A text field style with no decoration.

static var roundedBorder: RoundedBorderTextFieldStyle

A text field style with a system-defined rounded border.

static var squareBorder: SquareBorderTextFieldStyle

A text field style with a system-defined square border.

