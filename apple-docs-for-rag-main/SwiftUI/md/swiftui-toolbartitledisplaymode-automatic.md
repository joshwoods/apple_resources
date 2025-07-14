

- SwiftUI
- ToolbarTitleDisplayMode
-  automatic 

Type Property

# automatic

The automatic mode.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var automatic: ToolbarTitleDisplayMode { get }
```

## Discussion

For root content in a navigation stack in iOS, iPadOS, or tvOS this behavior will:

- Default to large when a navigation title is configured.

- Default to inline when no navigation title is provided.

In all platforms, content pushed onto a navigation stack will use the behavior of the content already on the navigation stack. This has no effect in macOS.

## See Also

### Getting display modes

static var inline: ToolbarTitleDisplayMode

The inline mode.

static var inlineLarge: ToolbarTitleDisplayMode

The inline large mode.

static var large: ToolbarTitleDisplayMode

The large mode.

