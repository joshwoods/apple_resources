

- AppKit
- NSMenu
- NSMenu.PresentationStyle
-  NSMenu.PresentationStyle.palette 

Case

# NSMenu.PresentationStyle.palette

A menu presentation style where items to display align horizontally.

macOS 14.0+

``` source
case palette
```

## Discussion

You can turn any menu into a palette menu by setting the menu’s presentation style to `.palette`. For each menu item, set its image. For template images, AppKit automatically adds the appropriate selection tint. Alternatively you can set the offStateImage and the onStateImage. Use the `onStateImage` to indicate selection.

The following example creates a presentation style menu that displays a list of sport images. When a menu item selects, the system automatically tints the image.

- Swift
- Objective-C

```
let parentMenu = NSMenu()

// Create a menu.
let paletteMenu = NSMenu()
let symbols = ["figure.barre", "figure.american.football", "figure.soccer", "figure.fishing", "figure.roll"]
for symbol in symbols {
    let item = NSMenuItem(title: symbol, action: nil, keyEquivalent: "")
    item.image = NSImage(systemSymbolName: symbol, accessibilityDescription: symbol)
    paletteMenu.addItem(item)
}

// Set the presentation style of the menu to palette.
paletteMenu.presentationStyle = .palette

// Create a menu item for the palette.
let paletteMenuItem = NSMenuItem()
paletteMenuItem.submenu = paletteMenu

// Create a menu and corresponding menu item to contain the palette menu item.
let menu = NSMenu(title: "Sports")
menu.addItem(.sectionHeader(title: "Sports Menu"))
menu.addItem(paletteMenuItem)

let menuItem = NSMenuItem()
menuItem.title = "Sports"
menuItem.submenu = menu

// Add the menu containing the palette to the parent menu.
parentMenu.addItem(menuItem)
```

```
NSMenu *parentMenu = [[NSMenu alloc] init];

// Create a menu.
NSMenu *paletteMenu = [[NSMenu alloc] init];
NSArray *symbols = @[@"figure.barre", @"figure.american.football", @"figure.soccer", @"figure.fishing", @"figure.roll"];
int index;
for(NSInteger index = 0; index 

## See Also

### Defining the menu style

case regular

The default presentation style for a menu.

