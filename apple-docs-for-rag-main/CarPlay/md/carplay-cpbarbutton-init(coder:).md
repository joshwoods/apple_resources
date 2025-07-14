

- CarPlay
- CPBarButton
-  init(coder:) 

Initializer

# init(coder:)

Creates a button initialized from data in the specified coder object.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init?(coder: NSCoder)
```

## Return Value

A new button.

## See Also

### Creating a CarPlay Bar Button

init(type: CPBarButton.Type, handler: CPBarButtonHandler?)

Creates a bar button with a type and handler.

Deprecated

init(image: UIImage, handler: CPBarButtonHandler?)

Creates a bar button that displays an image.

init(title: String, handler: CPBarButtonHandler?)

Creates a bar button that displays a text label.

enum Type

Types of bar buttons.

typealias CPBarButtonHandler

A block that CarPlay calls when the user taps a bar button.

