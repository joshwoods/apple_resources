

- SwiftUI
-  CommandMenu 

Structure

# CommandMenu

Command menus are stand-alone, top-level containers for controls that perform related, app-specific commands.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
struct CommandMenu where Content : View
```

## Mentioned in 

Grouping data with lazy stack views

## Overview

Command menus are realized as menu bar menus on macOS, inserted between the built-in View and Window menus in order of declaration. On iOS, iPadOS, and tvOS, SwiftUI creates key commands for each of a menu’s commands that has a keyboard shortcut.

## Topics

### Creating a command menu

init(_:content:)

Creates a new menu for a collection of app-specific commands, inserted in the standard location for app menus (after the View menu, in order with other menus declared without an explicit location).

## Relationships

### Conforms To

- Commands

## See Also

### Defining commands

func commands&lt;Content>(content: () -> Content) -> some Scene

Adds commands to the scene.

func commandsRemoved() -> some Scene

Removes all commands defined by the modified scene.

func commandsReplaced&lt;Content>(content: () -> Content) -> some Scene

Replaces all commands defined by the modified scene with the commands from the builder.

protocol Commands

Conforming types represent a group of related commands that can be exposed to the user via the main menu on macOS and key commands on iOS.

struct CommandGroup

Groups of controls that you can add to existing command menus.

struct CommandsBuilder

Constructs command sets from multi-expression closures. Like `ViewBuilder`, it supports up to ten expressions in the closure body.

struct CommandGroupPlacement

The standard locations that you can place new command groups relative to.

