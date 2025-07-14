

- CarPlay
-  CPBarButtonHandler 

Type Alias

# CPBarButtonHandler

A block that CarPlay calls when the user taps a bar button.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+

``` source
typealias CPBarButtonHandler = (CPBarButton) -> Void
```

## See Also

### Creating a CarPlay Bar Button

init?(coder: NSCoder)

Creates a button initialized from data in the specified coder object.

init(type: CPBarButton.Type, handler: CPBarButtonHandler?)

Creates a bar button with a type and handler.

Deprecated

init(image: UIImage, handler: CPBarButtonHandler?)

Creates a bar button that displays an image.

init(title: String, handler: CPBarButtonHandler?)

Creates a bar button that displays a text label.

enum Type

Types of bar buttons.

