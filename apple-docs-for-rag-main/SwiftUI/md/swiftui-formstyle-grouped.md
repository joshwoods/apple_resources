

- SwiftUI
- FormStyle
-  grouped 

Type Property

# grouped

A form style with grouped rows.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
static var grouped: GroupedFormStyle { get }
```

Available when `Self` is `GroupedFormStyle`.

## Discussion

Rows in a grouped rows form have leading aligned labels and trailing aligned controls within visually grouped sections.

## See Also

### Getting built-in form styles

static var automatic: AutomaticFormStyle

The default form style.

static var columns: ColumnsFormStyle

A non-scrolling form style with a trailing aligned column of labels next to a leading aligned column of values.

