

- WidgetKit
-  Preview(\_:as:using:widget:contentStates:) 

Macro

# Preview(\_:as:using:widget:contentStates:)

Preview a widget with an activity configuration, using the specified attributes and content states.

iOS 17.0+iPadOS 17.0+

``` source
@freestanding(declaration)
macro Preview(
    _ name: String? = nil,
    as viewKind: ActivityPreviewViewKind,
    using attributes: Attributes,
    widget: @escaping () -> Widget,
    @PreviewActivityBuilder contentStates: @escaping @MainActor () async -> [Attributes.ContentState]
) where Widget : Widget, Attributes : ActivityAttributes
```

## Parameters 

`name`  

An optional display name for the preview, which will appear in the canvas.

`viewKind`  

The kind of widget view to display.

`attributes`  

The attributes with which to configure the widget.

`widget`  

A closure producing the widget to be previewed.

`contentStates`  

A closure building the content states to be previewed.

## Mentioned in 

Previewing widgets and Live Activities in Xcode

## Overview

The preview will allow you to step through the specified content states and test out the transitions between states.

Note

The attributes must be of the type expected by the widget. (This will be enforced at run-time.)

