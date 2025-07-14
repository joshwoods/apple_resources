

- PencilKit
-  PKToolPickerCustomItem 

Class

# PKToolPickerCustomItem

An item that represents a custom tool in the tool picker.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
class PKToolPickerCustomItem
```

## Overview

A custom tool item represents a tool that isn’t one of the system tools. You configure details about a custom tool item yourself using PKToolPickerCustomItem.Configuration, including providing custom images to draw the body of the tool.

The following code shows how to create a tool picker with a custom tool item. This basic implementation of imageProvider retrieves an image for the tool body from an asset catalog. A full app might use a more advanced drawing implementation for the image provider, such as using UIGraphicsImageRenderer.

```
// Create a configuration for a custom tool item.
var config = PKToolPickerCustomItem.Configuration(identifier: "com.example.custom-tool", name: "My Tool")

// Provide a custom image for the custom tool item.
config.imageProvider = { toolItem in
    guard let toolImage = UIImage(named: config.name) else { 
        return UIImage() 
    }
    return toolImage
}

// Configure additional appearance options for the custom tool item.
config.allowsColorSelection = true
config.defaultColor = .red
config.defaultWidth = 10.0

// Create a custom tool item using the configuration.
let customItem = PKToolPickerCustomItem(configuration: config)

// Create a picker with the custom tool item and a system ruler tool.
let items = [customItem, PKToolPickerRulerItem()]
let picker = PKToolPicker(toolItems: items)
```

For a more complete example of creating a custom tool item, see Configuring the PencilKit tool picker.

## Topics

### Creating a custom item

convenience init(configuration: PKToolPickerCustomItem.Configuration)

Creates a new custom item with the specified configuration.

### Configuring the custom item

var color: UIColor

The current color of the custom tool item.

var width: CGFloat

The current width of the custom tool item.

var configuration: PKToolPickerCustomItem.Configuration

The configuration of the custom tool item.

struct Configuration

A configuration that specifies the appearance and behavior of a custom tool item and its contents.

### Reloading the custom item image

func reloadImage()

Requests a new image for the custom tool item from the image provider.

### Structures

struct ControlOptions

Options for which controls to present.

### Instance Properties

var allowsColorSelection: Bool

Present color selection UI to the user. Defaults to the value set in `configuration`.

## Relationships

### Inherits From

- PKToolPickerItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating a tool picker

init()

Creates a new tool picker with a default set of tools.

init(toolItems: [PKToolPickerItem])

Creates a new tool picker with the tools you specify.

class PKToolPickerInkingItem

An item that represents an inking tool in the tool picker.

class PKToolPickerEraserItem

An item that represents an eraser tool in the tool picker.

class PKToolPickerLassoItem

An item that represents a lasso tool in the tool picker.

class PKToolPickerRulerItem

An item that represents a ruler tool in the tool picker.

class PKToolPickerScribbleItem

An item that represents a Scribble tool in the tool picker.

class PKToolPickerItem

The base class for an item in the tool picker.

