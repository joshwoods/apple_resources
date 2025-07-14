

- SwiftUI
-  AsyncImagePhase 

Enumeration

# AsyncImagePhase

The current phase of the asynchronous image loading operation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum AsyncImagePhase
```

## Overview

When you create an AsyncImage instance with the init(url:scale:transaction:content:) initializer, you define the appearance of the view using a `content` closure. SwiftUI calls the closure with a phase value at different points during the load operation to indicate the current state. Use the phase to decide what to draw. For example, you can draw the loaded image if it exists, a view that indicates an error, or a placeholder:

```
AsyncImage(url: URL(string: "https://example.com/icon.png")) { phase in
    if let image = phase.image {
        image // Displays the loaded image.
    } else if phase.error != nil {
        Color.red // Indicates an error.
    } else {
        Color.blue // Acts as a placeholder.
    }
}
```

## Topics

### Getting load phases

case empty

No image is loaded.

case success(Image)

An image succesfully loaded.

case failure(any Error)

An image failed to load with an error.

### Getting the image

var image: Image?

The loaded image, if any.

### Getting the error

var error: (any Error)?

The error that occurred when attempting to load an image, if any.

## Relationships

### Conforms To

- Sendable

## See Also

### Loading images asynchronously

struct AsyncImage

A view that asynchronously loads and displays an image.

