

- SwiftUI
-  InspectorCommands 

Structure

# InspectorCommands

A built-in set of commands for manipulating inspectors.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
struct InspectorCommands
```

## Overview

`InspectorCommands` include a command for toggling the presented state of the inspector with a keyboard shortcut of ⌘⌃I.

These commands are optional and can be explicitly requested by passing a value of this type to the commands(content:) modifier:

```
@State var presented = true
WindowGroup {
    MainView()
        .inspector(isPresented: $presented) {
            InspectorView()
        }
}
.commands {
    InspectorCommands()
}
```

## Topics

### Creating a command

init()

A new value describing the built-in inspector-related commands.

## Relationships

### Conforms To

- Commands

## See Also

### Getting built-in command groups

struct SidebarCommands

A built-in set of commands for manipulating window sidebars.

struct TextEditingCommands

A built-in group of commands for searching, editing, and transforming selections of text.

struct TextFormattingCommands

A built-in set of commands for transforming the styles applied to selections of text.

struct ToolbarCommands

A built-in set of commands for manipulating window toolbars.

struct ImportFromDevicesCommands

A built-in set of commands that enables importing content from nearby devices.

struct EmptyCommands

An empty group of commands.

