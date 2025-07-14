

- SwiftUI
-  CommandGroupPlacement 

Structure

# CommandGroupPlacement

The standard locations that you can place new command groups relative to.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
struct CommandGroupPlacement
```

## Overview

The names of these placements aren’t visible in the user interface, but the discussion for each placement lists the items that it includes.

## Topics

### App interactions

static let appInfo: CommandGroupPlacement

Placement for commands that provide information about the app, the terms of the user’s license agreement, and so on.

static let appSettings: CommandGroupPlacement

Placement for commands that expose app settings and preferences.

static let appTermination: CommandGroupPlacement

Placement for commands that result in app termination.

static let appVisibility: CommandGroupPlacement

Placement for commands that control the visibility of running apps.

static let systemServices: CommandGroupPlacement

Placement for commands that expose services other apps provide.

### File manipulation

static let importExport: CommandGroupPlacement

Placement for commands that relate to importing and exporting data using formats that the app doesn’t natively support.

static let newItem: CommandGroupPlacement

Placement for commands that create and open different kinds of documents.

static let printItem: CommandGroupPlacement

Placement for commands related to printing app content.

static let saveItem: CommandGroupPlacement

Placement for commands that save open documents and close windows.

### Content updates

static let pasteboard: CommandGroupPlacement

Placement for commands that interact with the Clipboard and manipulate content that is currently selected in the app’s view hierarchy.

static let textEditing: CommandGroupPlacement

Placement for commands that manipulate and transform text selections.

static let textFormatting: CommandGroupPlacement

Placement for commands that manipulate and transform the styles applied to text selections.

static let undoRedo: CommandGroupPlacement

Placement for commands that control the Undo Manager.

### Bars

static let sidebar: CommandGroupPlacement

Placement for commands that control the app’s sidebar and full-screen modes.

static let toolbar: CommandGroupPlacement

Placement for commands that manipulate the toolbar.

### Windows

static let singleWindowList: CommandGroupPlacement

Placement for commands that describe and reveal any windows that the app defines.

static let windowArrangement: CommandGroupPlacement

Placement for commands that arrange all of an app’s windows.

static let windowList: CommandGroupPlacement

Placement for commands that describe and reveal the app’s open windows.

static let windowSize: CommandGroupPlacement

Placement for commands that control the size of the window.

### Help

static let help: CommandGroupPlacement

Placement for commands that present documentation and helpful information to people.

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

struct CommandMenu

Command menus are stand-alone, top-level containers for controls that perform related, app-specific commands.

struct CommandGroup

Groups of controls that you can add to existing command menus.

struct CommandsBuilder

Constructs command sets from multi-expression closures. Like `ViewBuilder`, it supports up to ten expressions in the closure body.

