

- WidgetKit
-  WidgetPreviewContext 

Structure

# WidgetPreviewContext

A specification for the context of a widget preview.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
struct WidgetPreviewContext
```

## Overview

To create a preview for a widget in Xcode, use previewContext(_:) and pass `WidgetPreviewContext` initialized with the appropriate `WidgetFamily`.

```
struct Widget_Previews: PreviewProvider {
    static var previews: some View {
        Group {
            MyWidgetView()
                .previewContext(WidgetPreviewContext(family: .systemSmall))
        }
    }
}
```

## Topics

### Creating a Preview Context

init(family: WidgetFamily)

Creates a context for previewing a widget or a widget’s view.

## Relationships

### Conforms To

- PreviewContext

## See Also

### Widget preview and debugging

Previewing widgets and Live Activities in Xcode

Use Xcode previews to iteratively develop, fine-tune, and troubleshoot widgets and Live Activities.

Debugging Widgets

Set environment variables in Xcode to control your widget’s configuration in the debugger.

Preview macros

Use Swift macros to create widget previews in Xcode.

