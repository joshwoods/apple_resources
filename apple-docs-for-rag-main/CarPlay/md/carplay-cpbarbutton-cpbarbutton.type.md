

- CarPlay
- CPBarButton
-  CPBarButton.Type 

Enumeration

# CPBarButton.Type

Types of bar buttons.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
enum `Type`
```

## Topics

### Button Types

case text

A text style bar button.

case image

An image style bar button.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

typealias CPBarButtonHandler

A block that CarPlay calls when the user taps a bar button.

