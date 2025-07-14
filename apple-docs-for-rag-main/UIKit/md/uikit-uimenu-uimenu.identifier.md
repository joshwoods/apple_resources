

- UIKit
- UIMenu
-  UIMenu.Identifier 

Structure

# UIMenu.Identifier

Constants you use to identify an app’s standard menus.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
struct Identifier
```

## Overview

Use these constants to identify UIMenu objects containing standard configurations.

When creating a custom menu identifier, provide a reverse domain name string value, such as `UIMenu.Identifier("com.example.apple-samplecode.MenubarSample.reloadMenu")`.

## Topics

### Top-level menus

static let application: UIMenu.Identifier

The standard app menu.

static let file: UIMenu.Identifier

The standard File menu.

static let edit: UIMenu.Identifier

The standard Edit menu.

static let view: UIMenu.Identifier

The standard View menu.

static let window: UIMenu.Identifier

The standard Window menu.

static let help: UIMenu.Identifier

The standard Help menu.

### App menu commands

static let about: UIMenu.Identifier

The About menu.

static let preferences: UIMenu.Identifier

The Preferences menu.

static let services: UIMenu.Identifier

The Services menu.

static let hide: UIMenu.Identifier

The Hide menu.

static let quit: UIMenu.Identifier

The Quit menu.

### File menus

static let newScene: UIMenu.Identifier

The New Scene menu.

static let openRecent: UIMenu.Identifier

The Open Recent menu.

static let open: UIMenu.Identifier

The Open menu.

static let close: UIMenu.Identifier

The Close menu.

static let print: UIMenu.Identifier

The Print menu.

static let document: UIMenu.Identifier

The Document menu.

### Edit menus

static let undoRedo: UIMenu.Identifier

The Undo/Redo menu.

static let standardEdit: UIMenu.Identifier

The standard Edit menu.

static let find: UIMenu.Identifier

The Find menu.

static let replace: UIMenu.Identifier

The Replace menu.

static let share: UIMenu.Identifier

The Share menu.

static let textStyle: UIMenu.Identifier

The Text Style menu.

static let spelling: UIMenu.Identifier

The Spelling menu.

static let spellingPanel: UIMenu.Identifier

The Spelling Panel menu.

static let spellingOptions: UIMenu.Identifier

The Spelling Options menu.

static let substitutions: UIMenu.Identifier

The Substitutions menu.

static let substitutionsPanel: UIMenu.Identifier

The Substitutions Panel menu.

static let substitutionOptions: UIMenu.Identifier

The Substitutions Options menu.

static let transformations: UIMenu.Identifier

The Transformations menu.

static let speech: UIMenu.Identifier

The Speech menu.

static let lookup: UIMenu.Identifier

The Lookup menu.

static let learn: UIMenu.Identifier

The Learn menu.

static let format: UIMenu.Identifier

The Format menu.

static let font: UIMenu.Identifier

The Font menu.

static let textSize: UIMenu.Identifier

The Text Size menu.

static let textColor: UIMenu.Identifier

The Text Color menu.

static let textStylePasteboard: UIMenu.Identifier

The Text Style Pasteboard menu.

static let text: UIMenu.Identifier

The Text menu.

static let autoFill: UIMenu.Identifier

The AutoFill menu.

static let writingDirection: UIMenu.Identifier

The Writing Direction menu.

static let alignment: UIMenu.Identifier

The Alignment menu.

### View menus

static let toolbar: UIMenu.Identifier

The Toolbar menu group.

static let sidebar: UIMenu.Identifier

The Sidebar menu group.

static let fullscreen: UIMenu.Identifier

The Full Screen menu.

### Window menus

static let minimizeAndZoom: UIMenu.Identifier

The Minimize and Zoom menu.

static let bringAllToFront: UIMenu.Identifier

The Bring All to Front menu.

### Root menu

static let root: UIMenu.Identifier

The root menu.

### Initializers

init(String)

Creates a menu identifier.

init(rawValue: String)

Creates a menu identifier with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a menu object

convenience init(title: String, image: UIImage?, identifier: UIMenu.Identifier?, options: UIMenu.Options, children: [UIMenuElement])

Creates a new menu with the specified values.

convenience init(title: String, subtitle: String?, image: UIImage?, identifier: UIMenu.Identifier?, options: UIMenu.Options, children: [UIMenuElement])

Creates a new menu with the specified title, subtitle, image, identifier, menu options, and child elements.

convenience init(title: String, subtitle: String?, image: UIImage?, identifier: UIMenu.Identifier?, options: UIMenu.Options, preferredElementSize: UIMenu.ElementSize, children: [UIMenuElement])

Creates a new menu with the specified title, subtitle, image, identifier, menu options, element size, and child elements.

struct Options

Options you use to configure a menu’s appearance.

init?(coder: NSCoder)

Creates a menu from data in an unarchiver.

