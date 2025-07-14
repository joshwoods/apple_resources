

- CarPlay
- CPBarButton
-  init(type:handler:) Deprecated

Initializer

# init(type:handler:)

Creates a bar button with a type and handler.

iOS 12.0–14.0DeprecatediPadOS 12.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
init(
    type: CPBarButton.Type,
    handler: CPBarButtonHandler? = nil
)
```

## Parameters 

`type`  

The button type.

`handler`  

The block that CarPlay invokes when the user taps the button.

## Return Value

A bar button of the specified type.

## See Also

### Creating a CarPlay Bar Button

init?(coder: NSCoder)

Creates a button initialized from data in the specified coder object.

init(image: UIImage, handler: CPBarButtonHandler?)

Creates a bar button that displays an image.

init(title: String, handler: CPBarButtonHandler?)

Creates a bar button that displays a text label.

enum Type

Types of bar buttons.

typealias CPBarButtonHandler

A block that CarPlay calls when the user taps a bar button.

