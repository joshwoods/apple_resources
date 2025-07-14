

- CarPlay
- CPBarButton
-  init(title:handler:) 

Initializer

# init(title:handler:)

Creates a bar button that displays a text label.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(
    title: String,
    handler: CPBarButtonHandler? = nil
)
```

## Parameters 

`title`  

The text to display on the button.

`handler`  

The block that CarPlay invokes when the user taps the button.

## Return Value

A bar button that displays the provided text.

## See Also

### Creating a CarPlay Bar Button

init?(coder: NSCoder)

Creates a button initialized from data in the specified coder object.

init(type: CPBarButton.Type, handler: CPBarButtonHandler?)

Creates a bar button with a type and handler.

Deprecated

init(image: UIImage, handler: CPBarButtonHandler?)

Creates a bar button that displays an image.

enum Type

Types of bar buttons.

typealias CPBarButtonHandler

A block that CarPlay calls when the user taps a bar button.

