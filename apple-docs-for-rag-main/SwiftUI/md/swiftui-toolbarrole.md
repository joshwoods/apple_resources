

- SwiftUI
-  ToolbarRole 

Structure

# ToolbarRole

The purpose of content that populates the toolbar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ToolbarRole
```

## Overview

A toolbar role provides a description of the purpose of content that populates the toolbar. The purpose of the content influences how a toolbar renders its content. For example, a browser will automatically leading align the title of a toolbar in iPadOS.

Provide this type to the toolbarRole(_:) modifier:

```
ContentView()
    .navigationTitle("Browser")
    .toolbarRole(.browser)
    .toolbar {
        ToolbarItem(placement: .primaryAction) {
            AddButton()
        }
     }
```

## Topics

### Behavior-specific roles

static var browser: ToolbarRole

The browser role.

static var editor: ToolbarRole

The editor role.

static var navigationStack: ToolbarRole

The navigationStack role.

### Automatic roles

static var automatic: ToolbarRole

The automatic role.

## Relationships

### Conforms To

- Sendable

## See Also

### Specifying the role of toolbar content

func toolbarRole(ToolbarRole) -> some View

Configures the semantic role for the content populating the toolbar.

