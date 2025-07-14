

- AppKit
- NSMenu
-  palette(colors:titles:template:onSelectionChange:) 

Type Method

# palette(colors:titles:template:onSelectionChange:)

Creates a palette style menu displaying user-selectable color tags that tint using the specified array of colors.

macOS 14.0+

``` source
static func palette(
    colors: [NSColor],
    titles: [String] = [],
    template: NSImage? = nil,
    onSelectionChange: ((NSMenu) -> Void)? = nil
) -> NSMenu
```

## Parameters 

`colors`  

The display colors for the menu items.

`titles`  

The menu item titles.

`template`  

The image the system displays for the menu items.

`onSelectionChange`  

The closure to invoke when someone selects the menu item.

## Return Value

A menu in the palette presentation style.

## Discussion

This factory method creates a presentation style menu as a selectable number of tags that display as colored circles or images. If `templateImage` is `nil`, a solid circle of color displays. If `templateImage` isn’t `nil`, the `templateImage` displays.

This code creates a menu with a group header and a palette menu. The palette menu display a solid circle for each color you pass into the `colors` parameter and adds a checkmark to the middle of the circle when you select the item. You can also optionally pass in a closure that executes when any selection changes.

```
let parentMenu = NSMenu()

// Create a palette styled menu using the factory method.
let colors: [NSColor] = [.systemRed, .systemOrange, .systemYellow, .systemGreen, .systemBlue]
let titles = ["red", "orange", "yellow", "green", "blue"]
let paletteMenu = NSMenu.palette(colors: colors, titles: titles) { menu in
    // Optionally add a closure to handle any selection changes.
    print("Currently selected colors: \(menu.selectedItems.map { $0.title })")
}

// Create a menu item for the palette and add the palette as a submenu.
let paletteMenuItem = NSMenuItem()
paletteMenuItem.submenu = paletteMenu

// Create a menu and corresponding menu item to contain the palette menu item.
let menu = NSMenu(title: "Colors")
menu.addItem(.sectionHeader(title: "Color Palette Menu"))
menu.addItem(paletteMenuItem)

let menuItem = NSMenuItem()
menuItem.title = "Colors"
menuItem.submenu = menu

// Add the menu containing the palette to the parent menu.
parentMenu.addItem(menuItem)
```

This code is similar to the previous example, only here the menu displays the `templateImage` of a flag tinted to the corresponding color you set in the `colors` array. When you select an item in this menu the image changes from a flag to a checkmark.

```
let parentMenu = NSMenu()

// Create a palette styled menu using the factory method.
let colors: [NSColor] = [.systemRed, .systemOrange, .systemYellow, .systemGreen, .systemBlue]
let titles = ["red", "orange", "yellow", "green", "blue"]
let template = NSImage(systemSymbolName: "flag.fill", accessibilityDescription: "flag")
let paletteMenu = NSMenu.palette(colors: colors, titles: titles, template: template) { menu in
    // Optionally add a closure to handle any selection changes.
    print("Currently selected flag colors: \(menu.selectedItems.map { $0.title })")
}

// Create a menu item for the palette and add the palette as a submenu.
let paletteMenuItem = NSMenuItem()
paletteMenuItem.submenu = paletteMenu

// Create a menu and corresponding menu item to contain the palette menu item.
let menu = NSMenu(title: "Flags")
menu.addItem(.sectionHeader(title: "Flags Palette Menu"))
menu.addItem(paletteMenuItem)

let menuItem = NSMenuItem()
menuItem.title = "Flags"
menuItem.submenu = menu

// Add the menu containing the palette to the parent menu.
parentMenu.addItem(menuItem)
```

When setting the `template` image favor images that tint (such as system images). Raster images don’t tint in this presentation style.

Menus that you create using this convenience method have a presentationStyle of type NSMenu.PresentationStyle.palette and a selectionMode of type NSMenu.SelectionMode.selectAny.

