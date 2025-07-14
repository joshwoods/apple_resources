

- SwiftUI
-  ToolbarTitleDisplayMode 

Structure

# ToolbarTitleDisplayMode

A type that defines the behavior of title of a toolbar.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ToolbarTitleDisplayMode
```

## Overview

Use the toolbarTitleDisplayMode(_:) modifier to configure the title display behavior of your toolbar:

```
NavigationStack {
    ContentView()
        .toolbarTitleDisplayMode(.inlineLarge)
}
```

## Topics

### Getting display modes

static var automatic: ToolbarTitleDisplayMode

The automatic mode.

static var inline: ToolbarTitleDisplayMode

The inline mode.

static var inlineLarge: ToolbarTitleDisplayMode

The inline large mode.

static var large: ToolbarTitleDisplayMode

The large mode.

## See Also

### Configuring the toolbar title display mode

func toolbarTitleDisplayMode(ToolbarTitleDisplayMode) -> some View

Configures the toolbar title display mode for this view.

