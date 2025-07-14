

- PencilKit
- PKToolPickerCustomItem
-  PKToolPickerCustomItem.Configuration 

Structure

# PKToolPickerCustomItem.Configuration

A configuration that specifies the appearance and behavior of a custom tool item and its contents.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
struct Configuration
```

## Topics

### Creating a configuration

init(identifier: String, name: String)

Create a new configuration with an identifier and a name.

### Identifying the custom tool

var identifier: String

A string that uniquely identifies the tool in the picker.

var name: String

A short string to show as the name of the tool in the UI.

### Customizing color

var defaultColor: UIColor

The default color for the tool.

var allowsColorSelection: Bool

A Boolean value that determines whether to show the color selection UI for the tool.

### Customizing width

var defaultWidth: CGFloat

The default width for the tool.

var widthVariants: [CGFloat : UIImage]

A dictionary with UI options for selecting width, with each element containing a width value and its corresponding image.

### Providing an image for the tool

var imageProvider: ((PKToolPickerCustomItem) -> UIImage)?

A closure to provide an image that represents the custom tool item.

### Providing a custom view controller for the tool

var viewControllerProvider: ((PKToolPickerCustomItem) -> UIViewController)?

A closure to provide a view controller above the system controls in the tool attributes popover.

### Instance Properties

var toolAttributeControls: PKToolPickerCustomItem.ControlOptions

Defines which attribute controls are available to be presented in UI such as the tool attributes popover, or inline in the picker presented from a pencil squeeze. Controls for properties which the tool item does not support will not be presented. Excluding a control here does not hide all UI for adjusting that value. For example, excluding the opacity control here will not remove it from the color picker, if the color picker is otherwise available. Defaults to all controls.

## See Also

### Configuring the custom item

var color: UIColor

The current color of the custom tool item.

var width: CGFloat

The current width of the custom tool item.

var configuration: PKToolPickerCustomItem.Configuration

The configuration of the custom tool item.

