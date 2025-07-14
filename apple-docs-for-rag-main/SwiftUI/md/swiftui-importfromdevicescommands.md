

- SwiftUI
-  ImportFromDevicesCommands 

Structure

# ImportFromDevicesCommands

A built-in set of commands that enables importing content from nearby devices.

macOS 12.0+

``` source
struct ImportFromDevicesCommands
```

## Overview

This set of commands adds items based on nearby devices and capabilities, like taking photos or scanning documents. Views can receive imported content from these menu items by using the importsItemProviders(_:onImport:) modifier.

These commands are optional and you can explicitly request them by passing a value of this type to the commands(content:) modifier.

## Topics

### Creating the command group

init()

Creates a new set of device import commands.

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

struct InspectorCommands

A built-in set of commands for manipulating inspectors.

struct EmptyCommands

An empty group of commands.

