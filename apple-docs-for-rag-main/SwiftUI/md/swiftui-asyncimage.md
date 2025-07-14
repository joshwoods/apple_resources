

- SwiftUI
-  AsyncImage 

Structure

# AsyncImage

A view that asynchronously loads and displays an image.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AsyncImage where Content : View
```

## Overview

This view uses the shared URLSession instance to load an image from the specified URL, and then display it. For example, you can display an icon that’s stored on a server:

```
AsyncImage(url: URL(string: "https://example.com/icon.png"))
    .frame(width: 200, height: 200)
```

Until the image loads, the view displays a standard placeholder that fills the available space. After the load completes successfully, the view updates to display the image. In the example above, the icon is smaller than the frame, and so appears smaller than the placeholder.

You can specify a custom placeholder using init(url:scale:content:placeholder:). With this initializer, you can also use the `content` parameter to manipulate the loaded image. For example, you can add a modifier to make the loaded image resizable:

```
AsyncImage(url: URL(string: "https://example.com/icon.png")) { image in
    image.resizable()
} placeholder: {
    ProgressView()
}
.frame(width: 50, height: 50)
```

For this example, SwiftUI shows a ProgressView first, and then the image scaled to fit in the specified frame:

Important

You can’t apply image-specific modifiers, like resizable(capInsets:resizingMode:), directly to an `AsyncImage`. Instead, apply them to the Image instance that your `content` closure gets when defining the view’s appearance.

To gain more control over the loading process, use the init(url:scale:transaction:content:) initializer, which takes a `content` closure that receives an AsyncImagePhase to indicate the state of the loading operation. Return a view that’s appropriate for the current phase:

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

### Loading an image

init(url: URL?, scale: CGFloat)

Loads and displays an image from the specified URL.

init&lt;I, P>(url: URL?, scale: CGFloat, content: (Image) -> I, placeholder: () -> P)

Loads and displays a modifiable image from the specified URL using a custom placeholder until the image loads.

### Loading an image in phases

init(url: URL?, scale: CGFloat, transaction: Transaction, content: (AsyncImagePhase) -> Content)

Loads and displays a modifiable image from the specified URL in phases.

## Relationships

### Conforms To

- View

## See Also

### Loading images asynchronously

enum AsyncImagePhase

The current phase of the asynchronous image loading operation.

