

- DeveloperToolsSupport
-  Preview 

Structure

# Preview

A base type that preview macros use to create previews.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor
struct Preview
```

## Overview

Frameworks like SwiftUI and WidgetKit define initializers for this type, along with framework-specific preview macros that rely on this type. You don’t use this type directly. Instead, use one of the preview macros, like Preview(_:body:).

## Topics

### Initializers

init&lt;Attributes>(String?, as: ActivityPreviewViewKind, using: Attributes, widget: () -> some Widget, contentStates: () async -> [Attributes.ContentState])

Creates a preview of a live activity widget.

init&lt;Provider>(String?, as: WidgetFamily, using: Provider.Intent, widget: () -> some Widget, timelineProvider: () -> Provider)

Creates a preview of a widget with an `AppIntent` configuration.

init&lt;Provider>(String?, as: WidgetFamily, using: Provider.Intent, widget: () -> some Widget, timelineProvider: () -> Provider)

Creates a preview of a widget with an `INIntent` configuration.

init(String?, as: WidgetFamily, widget: () -> some Widget, timeline: () async -> [any TimelineEntry])

Creates a preview of a timeline-style widget.

init(String?, as: WidgetFamily, widget: () -> some Widget, timelineProvider: () -> some TimelineProvider)

Creates a preview of a widget with a static configuration.

init(String?, immersionStyle: some ImmersionStyle, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> any View, cameras: () -> [PreviewCamera])

Creates a preview of a SwiftUI view in an immersive space with custom viewpoints.

init(String?, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> NSView)

Creates a preview of an NSView.

init(String?, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> NSViewController)

Creates a preview of an NSViewController.

init(String?, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> UIView)

init(String?, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> any View)

Creates a preview of a SwiftUI view.

init(String?, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> UIViewController)

init(String?, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> any View, cameras: () -> [PreviewCamera])

Creates a preview of a SwiftUI view using the specified traits and custom viewpoints.

init(String?, windowStyle: some WindowStyle, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> any View, cameras: () -> [PreviewCamera])

Creates a preview of a SwiftUI view in a window with custom viewpoints.

### Enumerations

enum ViewTraits

Traits that apply to previews of views and view controllers.

## Relationships

### Conforms To

- Sendable

## See Also

### Preview Registration

protocol PreviewRegistry

A protocol that the system uses to locate previews at runtime.

enum PreviewLayout

A size constraint for a preview.

struct PreviewTrait

Customizations that you can apply to a preview.

