

- TVML
- Layout Elements
-  menuBar 

# menuBar

Displays menu items along the top of the screen.

## Overview

Users can navigate left and right to move between `menuBar` elements. Here’s an example of a menu bar with two items inside of a `menuBarTemplate` element.

```

            Top Movies

            Genres

```

You can also add view elements to the left and right sides of the menu bar. The left `leadingAccessoryView` and right `trailingAccessoryView` can be any simple element, including Display Elements, Multimedia Elements, and Text Elements. Accessory views can also be row elements.

To add the equivalent of a leadingAccessoryView, add any supported element before the menuBar opening tag, as shown here:

```

            Top Movies

```

To add the equivalent of a trailingAccessoryView, add any supported element after the menuBar closing tag, as shown here:

```

            Top Movies

```

### Subelements of menuBar

- menuItem

- section

### Elements that Use menuBar

- mainTemplate

- menuBarTemplate

## Topics

### Valid TVML Style

tv-tint-color

Sets the tint color for an element.

### Valid TVML Attributes

binding

Associates information in a data item with an element.

prototype

Associates a data item type with an element.

theme

Sets the color scheme for an element.

## See Also

### Bar Elements

menuItem

Displays a label for an item.

nowPlayingMenuItem

Displays information about currently playing audio.

segmentBar

Displays a list of segment bar items.

segmentBarHeader

Displays information above a segment bar.

segmentBarItem

Provides titles inside of a segment bar.

tumblerBar

Displays a list of `tumblerItem` elements.

tumblerItem

Contains title information for a tumbler header.

