

- SwiftUI
-  CustomizableToolbarContent 

Protocol

# CustomizableToolbarContent

Conforming types represent items that can be placed in various locations in a customizable toolbar.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
protocol CustomizableToolbarContent : ToolbarContent where Self.Body : CustomizableToolbarContent
```

## Topics

### Using default options

func defaultCustomization() -> some CustomizableToolbarContent

Configures customizable toolbar content with the default visibility and options.

Deprecated

func defaultCustomization(Visibility, options: ToolbarCustomizationOptions) -> some CustomizableToolbarContent

Configures the way customizable toolbar items with the default behavior behave.

### Customizing the behavior

func customizationBehavior(ToolbarCustomizationBehavior) -> some CustomizableToolbarContent

Configures the customization behavior of customizable toolbar content.

### Instance Methods

func hidden(Bool) -> some CustomizableToolbarContent

Hides a toolbar item within its toolbar.

## Relationships

### Inherits From

- ToolbarContent

### Conforming Types

- Group

  Conforms when `Content` conforms to `CustomizableToolbarContent`.

- ToolbarItem

  Conforms when `ID` is `String` and `Content` conforms to `View`.

- ToolbarTitleMenu

## See Also

### Populating a customizable toolbar

func toolbar&lt;Content>(id: String, content: () -> Content) -> some View

Populates the toolbar or navigation bar with the specified items, allowing for user customization.

struct ToolbarCustomizationBehavior

The customization behavior of customizable toolbar content.

struct ToolbarCustomizationOptions

Options that influence the default customization behavior of customizable toolbar content.

